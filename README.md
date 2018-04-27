// # FootballProgram
// Selecting offensive plays based on the defensive look

let coverage = ['Man', 'Zone', 'Nickel', 'Blitz', 'Banjo'];
let down = [1, 2, 3, 4];
let distance = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
let offense = ['Play Action', 'HB Draw', 'Slip screen', 'Slants', 'Fly', 'Punt'];
let ranDown = down[Math.floor(Math.random() * down.length)];
let ranDistance = distance[Math.floor(Math.random() * distance.length)];
let ranCoverage = coverage[Math.floor(Math.random() * coverage.length)];

function playScenario(x, y, z) {
	console.log(ranDown, ranDistance, ranCoverage);
}

playScenario();
