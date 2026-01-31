<script>
    import nstrLogo from '../../figmaAssets/Logos/NSTR_White_Logo.svg'
    import kurmerLogo from '../../figmaAssets/Logos/kurmer.svg'
    import lanasionalLogo from '../../figmaAssets/Logos/LANasional.svg'
    import libraryBG from '../../backgrounds/library.png'
    import whiteKurmerLogo from '../../figmaAssets/Logos/Kurmer_Light.svg'
</script>

<div fetchpriority=high id="home">
    <div id="upperHalfDiv">
        <img id="nstrLogo" class="logo" src={nstrLogo} alt="Nusantara Pathway">
        <h1 id="upperHalfText">Nusantara Pathway</h1>
        <p>Jalur Matematika SMA Berorientasi Internasional</p>
    </div>
    <div id="lowerHalfDiv">
        <div class="lowerHalfDivLogo">
            <img id="kurmerLogo" class="logo" src={whiteKurmerLogo} alt="Kurikulum Merdeka">
            <img id="lanasionalLogo" class="logo" src={lanasionalLogo} alt="LANasional">
        </div>
        
    </div>
</div>

<style>
    * {
        margin: 0;
        padding: 0;
    }

    h1, p {
        text-align: right;
    }

    /* p {
        color: rgb(0, 0, 0);
    } */
    #home {
        color: white;
        width: 100%;
        height: calc(100vh - 58px);
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        
        background: url('../../backgrounds/graduate.jpg');
        background-size: cover;
        background-position: center;
    }

    #upperHalfDiv {
        padding-right: 2.5%;
        margin-top: 2%;

        display: flex;
        flex-direction: column;
        box-sizing: border-box;
        
        width: 100%;
        align-items:flex-end;
    }

    #upperHalfText {
        margin-top: 1.5%;
    }

    #lowerHalfDiv {
        padding-left: 2.5%;
        margin-bottom: 2%;

        display: flex;
        flex-direction: column;
        box-sizing: border-box;
        
        width: 100%;
        height: fit-content;
        align-items:flex-start;
    }

    .lowerHalfDivLogo {
        display: flex;
        width: 20%;
        margin-bottom: 1%;
    }

    #nstrLogo {
        width: 15%;
    }

    #kurmerLogo {
        width: 50%;
    }

    #lanasionalLogo {
        width: 50%;
    }

    @media only screen and (max-width: 720px) {
        #nstrLogo {
        width: 40%;
        }
        .lowerHalfDivLogo {
            width: 60%;
        }
    }


</style>