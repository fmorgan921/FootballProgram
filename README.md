// # FootballProgram
// Selecting offensive plays based on the defensive look
// Certain situations call for specific plays. Otherwise, the Quarterback has to come up with something!

let coverage = ['Man', 'Zone', 'Nickel', 'Blitz', 'Banjo'];
let down = [1, 2, 3, 4];
let distance = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
let offense = ['Play Action', 'HB Dive', 'Slip screen', 'Slants', 'Fly', 'Punt'];
let ranDown = down[Math.floor(Math.random() * down.length)];
let ranDistance = distance[Math.floor(Math.random() * distance.length)];
let ranCoverage = coverage[Math.floor(Math.random() * coverage.length)];
let quarterBack = 'Dak Prescott'

function playScenario(x, y, z) {
	console.log(ranDown, ranDistance, ranCoverage);
	if (ranDown === 1) {
		console.log(offense[1]);
	}
	else if (ranCoverage === 'Blitz') {
		console.log(offense[2]);
	}
	else if (ranDown === 2 && ranDistance <= 2 && ranCoverage != 'Blitz') {
		console.log(offense[0]);
	}
	else if (ranDown === 3 && ranDistance >= 8) {
		console.log(offense[4]);
	}
	else if (ranDistance <= 2) {
		console.log(offense[1]);
	}
	else if (ranDown === 4 && ranDistance > 2) {
		console.log(offense[5]);
	}
	else console.log('Come up with something, ' + quarterBack + '!');
}

playScenario();
