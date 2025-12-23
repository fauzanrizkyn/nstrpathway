<script>
    import nstrLogo from '../../figmaAssets/Logos/nstrpathway.svg'
    import kurmerLogo from '../../figmaAssets/Logos/kurmer.svg'
    import lanasionalLogo from '../../figmaAssets/Logos/LANasional.svg'
    import libraryBG from '../../backgrounds/library.png'
    
</script>

<div id="home">
    <div id="upperHalfDiv">
        <img id="nstrLogo" class="logo" src={nstrLogo} alt="Nusantara Pathway">
        <h1 id="upperHalfText">Nusantara Pathway</h1>
        <p>Jalur Matematika SMA Berorientasi Internasional</p>
    </div>
    <div id="lowerHalfDiv">
        <div class="lowerHalfDivLogo">
            <img id="kurmerLogo" class="logo" src={kurmerLogo} alt="Kurikulum Merdeka">
            <img id="lanasionalLogo" class="logo" src={lanasionalLogo} alt="LANasional">
        </div>
        <p>ⓒ Nusantara Pathway - 2026</p>
    </div>
</div>

<style>
    * {
        margin: 0;
        padding: 0;
    }
    #home {
        color: white;
        width: 100%;
        height: calc(100vh - 58px);
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        
        background: #30f830;
        background-size: cover;
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
        width: 50%;
        margin-bottom: 1%;
    }

    #nstrLogo {
        width: 15%;
    }

    #kurmerLogo {
        width: 15%;
    }


</style>