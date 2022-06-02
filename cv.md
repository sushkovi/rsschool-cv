# Hi my name is Vlad Sushko <img src="https://raw.githubusercontent.com/MartinHeinz/MartinHeinz/master/wave.gif" width="30px">

![Front-end dev.](./img/Cover.png)

## Contacts

- **Phone number** : <a href='tel:+375293635845'>+375293635845</a>
- **Discord** : MrCoobik#1974
- **GitHub** : https://github.com/sushkovi
- **My Website** : https://sushkovi.vercel.app/
- [![telegram](./img/telegram.svg)](https://t.me/sushko_vlad)
  [![linkedin](./img/linked-in.svg)](https://www.linkedin.com/in/vladsushko/)

---

## About me

I am a Front End developer. I decided to take courses for certificates and learn something new. I am already working in this area.

---

## Skills

### My Hard Skills :

- React
- TypeScript
- Redux Toolkit
- GraphQl
- React Native

### My Soft Skills:

- Communication Self-management
- Teamwork
- Negotiation and Conflict Resolution
- Flexibility Responsibility

## Code Example [Codewars](https://www.codewars.com/users/sushkovi)

```javascript
function validSolution(board) {
	let valid = true;
	const testvaliditiy = (arr) => {
		let set = new Set(arr);
		if (arr.includes(0) || [...set].length !== 9) {
			return false;
		} else {
			return true;
		}
	};

	console.log('row testing ...');
	for (i = 0; i < board.length; i++) {
		if (!valid) break;
		let row = [];
		for (j = 0; j < board.length; j++) {
			row.push(board[i][j]);
		}
		// console.log(row)
		valid = testvaliditiy(row);
	}

	//column testing
	console.log('Column testing ...');
	for (i = 0; i < board.length; i++) {
		let col = [];
		for (j = 0; j < board.length; j++) {
			col.push(board[j][i]);
		}
		valid = testvaliditiy(col);
		if (!valid) break;
	}

	//3x3 testing
	console.log('Cube 3x3 testing ...');
	let row = 0;
	let column = 0;
	while (row < 9 && column < 9) {
		let cube = [];
		for (i = row; i < row + 3; i++) {
			for (j = column; j < column + 3; j++) {
				cube.push(board[i][j]);
			}
		}
		row += 3;
		valid = testvaliditiy(cube);
		if (!valid) break;
		if (row == 9 && column != 9) {
			column += 3;
			row = 0;
		}
	}
	return valid;
}
```

## Education

**Belarusian State Pedagogical University Named after Maxim Tank (BSPU)**

## Languages

English - A2 > B1
Russian - Native
