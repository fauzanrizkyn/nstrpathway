<script>
	import AboutInfo from '../../figmaAssets/Logos/AboutInfo.svg';
</script>

<div id="about">
	<div id="aboutMain" class="halfHorizontal">
		<div class="halfVertical">
			<h2>Selamat Datang di</h2>
			<div id="nstrTitle">
				<h1>Nusantara</h1>
				<h1>Pathway</h1>
			</div>
		</div>
		
	</div>
	<div id="aboutDescriptionContainer" class="halfHorizontal">
		<div id="aboutDescription" class="halfHorizontal">
			<p id="aboutLeadParagraph">
				Nusantara Pathway merupakan program pendidikan menengah yang dirancang untuk memberikan
				jalur akademik yang terstruktur bagi siswa Indonesia yang berorientasi pada pendidikan
				tinggi internasional.
			</p>
			<p>
				Program ini dikembangkan sejak tahun 2023 dengan mengintegrasikan penguatan fondasi
				akademik, standar asesmen internasional, serta pembinaan keterampilan berpikir kritis dan
				kemandirian belajar yang dibutuhkan pada jenjang universitas.
			</p>
			<p>
				Melalui pendekatan kurikulum yang terarah, sistem asesmen berbasis kriteria, dan
				pendampingan akademik yang berkelanjutan, Nusantara Pathway membantu siswa membangun
				kesiapan akademik dan non-akademik untuk melanjutkan studi ke luar negeri secara bertahap
				dan realistis.
			</p>
		</div>
	</div>
</div>

<style>
	#about {
		width: 100%;
		height: 65vh;

		display: flex;
		flex-direction: row;
	}

	.halfHorizontal {
		width: 50%;
		height: 100%;
	}

	.halfVertical {
		width: 100%;
		height: 50%;
	}

	#aboutMain,
	#aboutDescriptionContainer {
		padding: 50px 0 50px 50px;
	}

	#aboutMain {
		display: flex;
		height: 85%;
	}

	#nstrTitle {
		margin-top: 2%;
	}

	#aboutDescriptionContainer {
		padding-right: 50px;
		width: 50%;
		height: 85%;
		display: flex;
		flex-direction: column;

		justify-content: flex-start;
	}

	#aboutDescription {
		width: 100%;
		height: 100%;

		display: flex;
		flex-direction: column;
		justify-content: space-between;
	}

	#aboutLeadParagraph {
		font-weight: 700;
	}

	@media only screen and (max-width: 720px) {
		.halfHorizontal {
			width: 100%;
			height: 100%;
		}

		.halfVertical {
			height: 50%;
		}
		
		#about {
			flex-direction: column;
			height: fit-content;

			padding-left: 1.5%;
			padding-top: 58px;
		}

		#aboutMain {
			display: flex;
			flex-direction: column;
			height: fit-content;
		}

		#nstrTitle {
			display: flex;
			flex-direction: row;
			gap: 3%;
		}

		#aboutDescriptionContainer {
			width: 100%;
			height: fit-content;
		}

		#aboutDescription {
			width: 100%;
			height: 100%;

			display: flex;
			flex-direction: column;
			gap: 3vh;
		}

	}
</style>
