// # FootballProgram
// Selecting offensive plays based on the defensive look
// Certain situations call for specific plays. Otherwise, the Quarterback has to come up with something!

let coverage = ['Man', 'Zone', 'Nickel', 'Blitz', 'Banjo'];
let down = Math.floor(Math.random() * 4 + 1);
let distance = Math.floor(Math.random() * 10 + 1);
let offense = ['Play Action', 'HB Dive', 'Slip screen', 'Slants', 'Fly', 'Punt'];
let ranCoverage = coverage[Math.floor(Math.random() * coverage.length)];
let quarterBack = 'Dak Prescott'

function playScenario() {
	console.log(down, distance, ranCoverage);
	if (down === 1) {
		console.log(offense[1]);
	}
	else if (ranCoverage === 'Blitz' && down != 4) {
		console.log(offense[2]);
	}
	else if (down === 2 && distance <= 2 && ranCoverage != 'Blitz') {
		console.log(offense[0]);
	}
	else if (down === 3 && distance >= 8) {
		console.log(offense[4]);
	}
	else if (distance <= 2) {
		console.log(offense[1]);
	}
	else if (down === 4 && distance > 2) {
		console.log(offense[5]);
	}
	else console.log('Come up with something, ' + quarterBack + '!');
}

playScenario();
