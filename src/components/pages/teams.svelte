<div id="teams">
	<h2>Tim Nusantara</h2>
	<div class="teamsCarousel">
		<div class="personEntry">
			<div id="Nukumizu" class="profilePic"></div>
			<div class="profileDesc">
				<h5>John Doe</h5>
				<p>
					Lorem ipsum dolor sit amet consectetur adipisicing elit. Aliquam illo a quod odit. Quos
					sint, est commodi fuga quam aut, sed eveniet voluptatibus ducimus.
				</p>
			</div>
		</div>
        <div class="personEntry">
			<div id="Nukumizu" class="profilePic"></div>
			<div class="profileDesc">
				<h5>John Doe</h5>
				<p>
					Lorem ipsum dolor sit amet consectetur adipisicing elit. Aliquam illo a quod odit. Quos
					sint, est commodi fuga quam aut, sed eveniet voluptatibus ducimus.
				</p>
			</div>
		</div>
	</div>
</div>

<style>
	#teams {
		padding: 2% 0 2% 0;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
	}
    h2 {
        text-align: center;
    }
	.teamsCarousel {
		margin-top: 25px;
		display: flex;
        gap: 20px;
	}

	.personEntry {
        width: 16vw;
		
		display: flex;
		flex-direction: column;
		border: 0.1px solid rgb(200, 200, 200);
        
	}

	.profileDesc {
		height: 30%;
        padding: 0 2% 0 2%;
	}

	.profilePic {
        width: 16vw;
        aspect-ratio: 9 / 16;
		height: 70%;
		background-position: center;
		background-size: cover;
		background-repeat: no-repeat;
	}

	#Nukumizu {
		background-image: url('../../backgrounds/person_single.webp');
	}
</style>
