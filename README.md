// # FootballProgram
// Selecting offensive plays based on the defensive look

let coverage = ['Man', 'Zone', 'Nickel', 'Blitz', 'Banjo'];
let offense = ['Play Action', 'HB Draw', 'Slip screen', 'Slants', 'Fly', 'Punt'];

for (let coverageIndex = 0; coverageIndex < coverage.length; coverageIndex++) {
	if (coverage[coverageIndex] === 'Man' || coverage[coverageIndex] === 'Banjo')
		console.log(offense[4]);
	else if (coverage[coverageIndex] === 'Blitz' || coverage[coverageIndex] === 'Zone')
		console.log(offense[2]);
	else if (coverage[coverageIndex] === 'Nickel')
		console.log(offense[0]);
	else console.log('Come up with something, Dak');
	}
