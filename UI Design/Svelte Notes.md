- $state - creates reactive variable that automatically updates the ui when it changes 
	- let count = $state(0);

- $derive - takes a reactive variable to compute a new value. is memoized, meaning it only changes when the reactive variable/dependency changes
	- let doubled = $derived(count * 2)

- $effect - runs some code/function when its dependency changes. any referenced variable inside the code will rerun the effect when there's a change
	- $effect(() => {
		- console.log("count changed to: ", count);
	- })

- $props - define inputs to a component
	- let  {myProp} = $props();