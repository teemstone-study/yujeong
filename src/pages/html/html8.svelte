<style>
	body,
	.calTop,
	.calBottom {
		display: flex;
	}

	body {
		flex-direction: column;
		width: 400px;
		height: 500px;
	}

	form {
		display: flex;
		width: 100%;
		height: 150px;
		flex-wrap: wrap;
		align-items: flex-end;
		padding-bottom: 10px;
		border: 1px solid red;
	}

	input {
		font-size: 30px;
		text-align: right;
		overflow: hidden;
	}

	input:focus {
		outline: none;
	}
	.result {
		display: flex;
		flex-wrap: wrap;
		width: 400px;
	}

	.calcPad1 {
		display: flex;
		flex-direction: column;
	}

	.calcSign {
		display: flex;
	}

	.calcSign ul {
		display: flex;
	}

	calcSign ul li {
		display: flex;
	}

	.funcKeytop,
	.numbKey,
	.funcKeyRight {
		width: 100px;
		height: 100px;
		border: 1px solid black;
		font-size: 35px;
		line-height: 0;
	}

	.funcKeytop button {
		background-color: #a5a5a5;
	}

	.funcKeytop button:active {
		background-color: white;
	}
	.calcSign button :hover::before {
		background-color: #a5a5a5;
	}

	.padRow1 {
		display: flex;
		flex-wrap: wrap;
	}

	.padRow2 {
		display: flex;
		flex-direction: row;
		width: 300px;
	}

	.padRow2 .numbKey {
		display: flex;
		align-items: center;
		/* padding-left: 15%; */
		width: 200px;
		/* border-radius: 50px; */
	}

	.padRow2 .numbKey .num0 {
		display: flex;
		align-items: center;
		margin: 2%;
		padding-left: 15%;
		width: 200px;
		border-radius: 50px;
	}
	.padRow2 .decimalPoint {
		display: flex;
		justify-content: center;
		align-items: center;
		width: 90px;
	}

	.numbKey button {
		background-color: #333333;
		color: white;
		position: relative;
	}
	.numbKey button:active::after {
		/* background-color: rgba(255, 255, 255, 0.8); */
		/* background: red; */
		/* position: absolute; */
		/* border-radius: 50%; */
		/* top: 0; */
		/* left: 0; */
		/* width: 100%; */
		/* height: 100%; */
		/* content: ''; */
	}

	.numbKey button:active {
		background-color: #545454;
	}

	.funcKeyRight button {
		background-color: #fe9f0c;
		color: white;
	}

	.funcKeyRight button:active {
		background-color: white;
		color: #fe9f0c;
	}
	ul li {
		display: flex;
		justify-content: center;
		align-items: center;
	}
	ul li button {
		width: 90px;
		height: 90px;
		border-radius: 50%;
		border: 1px solid black;
	}
</style>

<main>
	<body>
		<!-- result -->
		<div class="calTop">
			<form>
				<input class="result" type="text" />
			</form>
		</div>

		<!-- keyPad -->
		<div class="calBottom">
			<div class="calcPad1">
				<div class="calcSign">
					<ul>
						<li class="funcKeytop"><button class="allClear">AC</button></li>
						<li class="funcKeytop"><button class="plusMinus">±</button></li>
						<li class="funcKeytop"><button class="percentage">%</button></li>
					</ul>
				</div>
				<div class="keyPad">
					<ul>
						<div class="padRow1">
							<li class="numbKey"><button class="num7">7</button></li>
							<li class="numbKey"><button class="num8">8</button></li>
							<li class="numbKey"><button class="num9">9</button></li>
							<li class="numbKey"><button class="num4">4</button></li>
							<li class="numbKey"><button class="num5">5</button></li>
							<li class="numbKey"><button class="num6">6</button></li>
							<li class="numbKey"><button class="num1">1</button></li>
							<li class="numbKey"><button class="num2">2</button></li>
							<li class="numbKey"><button class="num3">3</button></li>
						</div>
						<div class="padRow2">
							<li class="numbKey"><button class="num0">0</button></li>
							<li class="numbKey"><button class="decimalPoint">.</button></li>
						</div>
					</ul>
				</div>
			</div>
			<div class="calcPad2">
				<div class="elementary4">
					<ul>
						<li class="funcKeyRight"><button class="divi">÷</button></li>
						<li class="funcKeyRight"><button class="multi">×</button></li>
						<li class="funcKeyRight"><button class="minus">－</button></li>
						<li class="funcKeyRight"><button class="plus">＋</button></li>
						<li class="funcKeyRight"><button class="equal">＝</button></li>
					</ul>
				</div>
			</div>
		</div>
	</body>
</main>
