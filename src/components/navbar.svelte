<script>
	import NusantaraPLogo from '../figmaAssets/Logos/NSTR_Outlined_Logo.svg';
	import Hamburger from '../figmaAssets/Other/Hamburger.svg';
	import HamburgerSad from '../figmaAssets/Other/HamburgerSad.svg'

    let navbarMobile;
    let navbarStatus = "closed"
    
    let hamburgir;
	let hamburgirSad;

	const navbarTrigger = () => {
        if (navbarStatus == "closed") {
            navbarMobile.style.opacity = "100%"
            navbarStatus = "open"
            
            hamburgir.style.transform = "rotate(180deg)"
			hamburgir.style.filter = "blur(10px)"
			hamburgir.style.opacity = 0

			hamburgirSad.style.opacity = 1
			hamburgirSad.style.transform = "rotate(180deg)"
        }
		else {
            navbarMobile.style.opacity = "0%"
            navbarStatus = "closed"

            hamburgir.style.transform = "rotate(0deg)"
			hamburgir.style.opacity = 1
			hamburgir.style.filter = "blur(0px)"

			hamburgirSad.style.opacity = 0
			hamburgirSad.style.transform = "rotate(0deg)"
        }

		//HEY ANTEK ANTEK ASHINGGG !n!
	};
</script>

<div id="navbarSpace"></div>
<div id="navbar">
	<img class="navbarItems" id="NusantaraLogo" src={NusantaraPLogo} alt="nusantar pathway" />
	<div class="navbarItems" id="links">
		<a href="./">Home</a>
		<a href="./#about">About</a>
		<a href="./#roadmap">Roadmap</a>
		<a href="./#approach">Approach</a>
	</div>
</div>
<div id="navbarMobile">
	
		<img class="navbarItems" id="NusantaraLogo" src={NusantaraPLogo} alt="nusantar pathway" />
		<button id="plate" on:click={navbarTrigger}>
			<img class="navbarButton" bind:this={hamburgir} id="hamburger" src={Hamburger} alt="hamburgir :)" />
			<img class="navbarButton" bind:this={hamburgirSad} id="hamburgerSad" src={HamburgerSad} alt="hamburgir :(" />
		</button>
</div>
<div bind:this={navbarMobile} class="navbarItems" id="linksMobile">
		<a on:click={navbarTrigger} href="./">Home</a>
		<a on:click={navbarTrigger} href="./#about">About</a>
		<a on:click={navbarTrigger} href="./#roadmap">Roadmap</a>
		<a on:click={navbarTrigger} href="./#approach">Approach</a>
	</div>

<style>
	* {
		padding: 0;
		margin: 0;
	}

	#navbarSpace {
		height: 58px;
	}

	#navbar {
		background-color: #f0f0f0;
		display: flex;
		position: fixed;
		flex-direction: row;
		align-items: center;
		justify-content: space-between;
		width: 100%;
		height: 58px;
		padding: 10px 2.5% 10px 2.5%;
		margin: 0;

		box-sizing: border-box;
	}

	#navbarMobile {
		display: none;
	}

	.navbarItems {
		height: 100%;
	}

	#links {
		display: flex;
		flex-direction: row;
		gap: 20px;
		height: 100%;
		justify-content: space-between;
	}

    #linksMobile {
        display: none;
    }

	a {
		text-decoration: none;
		color: black;
		display: flex;
		justify-content: center;
		align-items: center;

		scale: 1.1;
	}

	@media only screen and (max-width: 720px) {
        * {
            transition: all 0.25s ease-out;
        }

        button {
            border: none;
        }
		#navbarMobile {
            position: fixed;
			background-color: #f0f0f0;
			display: flex;
			flex-direction: row;
			align-items: center;
			justify-content: space-between;
			width: 100%;
			height: 58px;
			padding: 10px 2.5% 10px 2.5%;
			margin: 0;
			box-sizing: border-box;
		}

        .navbarButton {
			height: 100%;
			position: absolute;
		}

		#plate {
			position: relative;
		}

		#hamburger {
			right: 100%;
			top: 0;
		}

		#hamburgerSad {

			right: 100%;
			top: 0;
			z-index: -1;
		}

		#navbar {
			display: none;
		}

        #linksMobile {
            flex-direction: column;
            justify-content: center;
            gap: 50px;
            height: calc(100vh - 58px);
            background-color: #d1d0d0;

            position: fixed;
            opacity: 0%;
            width: 100%;
            margin-top: 58px;
            display: flex;
        }

        a {
            scale: 2;
        }

		button {
			height: 100%;
		}

		img {
			width: fit-content;
		}
	}
</style>
