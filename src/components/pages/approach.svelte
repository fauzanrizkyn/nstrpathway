<div id="approach">
	<div id="Teacher" class="approachEntry approachBG"></div>
	<div class="approachEntry approachText">
		<h3>Pendekatan Pendidikan</h3>
		<h1>Nusantara</h1>
		<h1>Pathway</h1>
		<p>
			Kami meyakini bahwa pendidikan yang efektif hanya dapat terwujud ketika kurikulum,
			pembelajaran, dan asesmen berjalan selaras. Nusantara Pathway dikembangkan dengan pendekatan
			bertahap yang menyeimbangkan pemahaman konsep, penerapan nyata, dan pengukuran kemajuan
			belajar yang adil, sehingga peserta didik tidak hanya unggul secara akademik, tetapi juga siap
			menghadapi pendidikan tinggi dan tantangan global.
		</p>
	</div>
	<div id="lowerApproachText" class="approachEntry approachText">
		<h2>“Pendidikan seharusnya membangun cara berpikir, bukan sekadar mengejar nilai.”</h2>
		<p>
			Nusantara Pathway menempatkan pemahaman, konsistensi, dan perkembangan peserta didik sebagai
			inti dari proses belajar.
		</p>
	</div>
	<div id="secondImage" class="approachEntry approachBG"></div>
	<div id="lowerApproachTextMobile" class="approachEntry approachText">
		<h2>“Pendidikan seharusnya membangun cara berpikir, bukan sekadar mengejar nilai.”</h2>
		<p>
			Nusantara Pathway menempatkan pemahaman, konsistensi, dan perkembangan peserta didik sebagai
			inti dari proses belajar.
		</p>
	</div>
</div>

<style>
	/* * {
		border: 1px solid red;
	} */

	p {
		width: 50%;
	}

	h2 {
		width: 60%;
	}
	#approach {
		display: grid;
		grid-template-columns: repeat(2, 1fr);
		width: 100%;
		height: auto;
		
	}

	#secondImage {
		background: url('../../backgrounds/rubikcube-student.png');
		background-size: cover;
		background-position: center;
		background-repeat: no-repeat;
	}

	#lowerApproachTextMobile {
		display: none;
	}

	#Teacher {
		background: url('../../backgrounds/aproach-1.webp');
		background-size: cover;
		background-position:bottom;
		background-repeat: no-repeat;
	}

	.approachEntry {
		width: 100%;
		height: 100vh;
	}

	.approachText {
		display: flex;
		flex-direction: column;
		justify-content: center;
		padding: 5% 0% 5% 5%;

		gap: 15px;
	}

	@media only screen and (max-width: 1020px) {
		
		#approach {
			display: flex;
			flex-direction: column;
		}

		#lowerApproachText {
			display: none;
		}

		#lowerApproachTextMobile {
			display: flex;
			justify-content: flex-start;
			padding-top: 5%;
		}

		p {
			width: 100%;
		}

		h2 {
			width: 100%;
		}

		.approachEntry {
		width: 100%;
		height: 70vh;
		}

		.approachText {
			width: 95%;
			height: 75%;
		}

		.approachBG {
			height: 50vh;
		}
	}
</style>
