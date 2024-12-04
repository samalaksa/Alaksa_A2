<script>
    import Todo from './Todo.svelte';
    import '../app.css';
    import underline from "$lib/img/underline.png"
</script>

    <h2 class="tracking-in-expand-fwd">Self Care</h2>
    <img class="underline " src="{underline}" alt="trash"/>
    <h1 class="tracking-in-expand-fwd">TO DO LIST</h1>

<Todo />

<style>
.tracking-in-expand-fwd {
    -webkit-animation: tracking-in-expand-fwd 1s cubic-bezier(0.215, 0.610, 0.355, 1.000) 1s both;
	animation: tracking-in-expand-fwd 1s cubic-bezier(0.215, 0.610, 0.355, 1.000) 1s both;
}
@-webkit-keyframes tracking-in-expand-fwd {
  0% {
    letter-spacing: -0.5em;
    -webkit-transform: translateZ(-700px);
            transform: translateZ(-700px);
    opacity: 0;
  }
  40% {
    opacity: 0.6;
  }
  100% {
    -webkit-transform: translateZ(0);
            transform: translateZ(0);
    opacity: 1;
  }
}
@keyframes tracking-in-expand-fwd {
  0% {
    letter-spacing: -0.5em;
    -webkit-transform: translateZ(-700px);
            transform: translateZ(-700px);
    opacity: 0;
  }
  40% {
    opacity: 0.6;
  }
  100% {
    -webkit-transform: translateZ(0);
            transform: translateZ(0);
    opacity: 1;
  }
}
.underline {
    width: 350px;
    max-width: 100%;
    height: auto;
    opacity: 30%;
}
</style>