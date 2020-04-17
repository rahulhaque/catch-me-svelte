<script>
  let flip = true;
  const run = (event) => {
    let randX = Math.floor(Math.random() * ((window.innerWidth - 150)/2));
		let randY = Math.floor(Math.random() * ((window.innerHeight - 150)/2));
    event.target.style.transform = flip ? 'scaleX(-1)' : 'scaleX(1)'; flip = !flip;
		event.target.style.left = randX + "px";
		event.target.style.top = randY + "px";
  }
</script>

<style>
  img {
    position: absolute; /* Important for element to move */
		top: 20px;
		left: 20px;
		transition: 0.5s;
  }
</style>

<img on:click={() => {alert('Gotcha!!! 👏')}} on:mouseover={event => run(event)} alt='lol' src='./assets/lol.png' height='100px'/>
