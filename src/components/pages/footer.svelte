<script>
	import Logo from '../../figmaAssets/Logos/NSTR_White_Logo.svg';
	import EmailLogo from '../../figmaAssets/Logos/email.png';
</script>

<div id="footer">
	<div id="footerContainer">
		<div id="footerDesc" class="footerEntry">
			<img src={Logo} alt="NusantaraLogo" />
			<p id="footerDescText">
				Nusantara Pathway merupakan program pendidikan menengah yang dirancang untuk memberikan
				jalur akademik yang terstruktur bagi siswa Indonesia yang berorientasi pada pendidikan
				tinggi internasional.
			</p>
		</div>
		<div class="footerEntry">
			<div class="footerInput">
				<h2 id="footerInputDesc">Tertarik dengan Nusantara Pathway?</h2>
				<div class="input">
					<input type="text" placeholder="someone@example.com" />
                    <a href="mailto:someone@example.com">
                        <button id="send">
						<img id="sendButton" src={EmailLogo} alt="Email Logo" />
					</button>
                    </a>
					
				</div>
			</div>
		</div>
		<div class="footerEntry">footer 3</div>
	</div>
</div>

<style>
	#footer {
		width: 100%;
		background: black;
		color: white;
		padding: 20px 10px;

		display: flex;
		justify-content: center;
	}

	#footerContainer {
		width: 90%;
		display: grid;
		grid-template-columns: repeat(3, 1fr);
		gap: 20px;
	}

	#footerDesc {
		display: flex;
		flex-direction: column;
		gap: 15px;
	}

	#footerDescText {
		width: 90%;
	}

	.footerEntry {
		width: 100%;
        height: 100%;
        box-sizing: border-box;
		/* border: 1px solid red; */
	}

	.footerInput {
		display: flex;
		flex-direction: column;
		height: 100%;
        justify-content: space-evenly;
	}

	.input {
		height: 25%;
        width: 90%;
		display: flex;
		flex-direction: row;
		background-color: white;
		border-radius: 50px;
	}

    #footerInputDesc {
        transform: translateY(20%);
    }

	input {
		background-color: transparent;
		width: 85%;
		height: 100%;
		text-align: center;
		font-size: 200%;
		border: none;

		font-family: 'Inter', sans-serif;
		font-optical-sizing: auto;
		font-style: normal;
	}

	input:focus {
		border: none;
		outline: none;
	}

	#send {
		border: none;
		border-radius: 50px;
		height: 100%;
		scale: 1.1;
	}

	#sendButton {
		width: 100%;
		height: 100%;
	}

	img {
		width: 70%;
	}

	p {
		font-weight: 100;
	}
</style>
