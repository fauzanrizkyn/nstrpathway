<script>
	import AboutInfo from '../../figmaAssets/Logos/AboutInfo.svg';
</script>

<div id="about">
			<h2>Selamat Datang di Nusantara Pathway</h2>
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

<style>
	#about {
		width: 100%;
		height: fit-content;

		display: flex;
		flex-direction: column;
		padding: 1% 2.5% 1% 2.5%;
		text-align: center;
		align-items: center;
	}

	p {
		margin-top: 0.5%;
		width: 50%;
		text-align: justify;
	}

	#aboutLeadParagraph {
		margin-top: 2%;
		font-weight: 700;
	}

	@media only screen and (max-width: 720px) {
		
		#about {
			flex-direction: column;
			height: fit-content;
			padding: 3% 2.5% 3% 2.5%;
			
		}

		p {
			width: 80%;
		}
	}
</style>
