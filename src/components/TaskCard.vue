
              
<template>
	<!-- task card in team page -->
  <div class='teamtask'>
    <div class = "taskDisplay"> Task </div>
    <div id = "taskName"> {{Task}} </div>
    <br>
    <div class = "taskDisplay"> Description </div>
    <div id = "taskDescription"> {{Description}} </div>
    <br>
	<div class = "taskDisplay"> Assigner </div>
	<div id = "taskAssigner"> {{Assigner}} </div>
	<br>
    <div id = "taskDuedate"> {{DueDate }}</div>
  </div>
  
</template>

<script>
 
 export default {
	name: 'TaskCard',
	props: {
		Task: {
			type: String,
		},
		Description: {
			type: String,
		},
		DueDate: {
			type: String
		},
		Assigner: {
			type: String
		}
	},
  };

</script>


<style>
 
 .teamtask {
	cursor: default;
	 background-color: var(--white);
	 padding: 1rem;
	 border-radius: 8px;
	 width: 450px;
	 box-shadow: rgba(99, 99, 99, 0.1) 0px 2px 8px 0px;
	 margin-bottom: 1rem;
	 border: none;
	 font-weight: 500;
}
 .teamtask p {
	 font-size: 14px;
	 
	 
}
 .taskDisplay {
  	background: transparent;
	border: 0;
	color: var(--text);
	font-size: 15px;
   	text-decoration-line: underline;
}

 #taskName, #taskDescription, #taskAssigner {
	 background: transparent;
	 border: 0;
	 color: var(--text);
	 font-size: 15px;
}
 #taskDuedate {
	position: relative;
	width: 85px;
   	
   	padding: 5px;
	color: var(--text);
	font-size: 12px;
	margin-right: 1rem;
   	border: 1px solid var(--light-grey);
   	border-radius: 3px;
	display: inline-block;
   
}

</style>