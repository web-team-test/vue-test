<template>
  <div class="task-manager">
    <div class="task-header">
      <h1>{{ msg }}</h1>
      <img alt="Task Manager" src="/assets/task.gif">
    </div>
    <div class="task-body">
      <h2>Objectives:</h2>
      <p>Create an app to add and remove To-Do tasks:</p>
      <ol>
        <li>
          <b>"Display Task List"</b> Create a To-Do task list that displays all Tasks in a list format, each task can be selected and removed.
          A 'Done' counter should be displayed below the list.
          If the list is empty then display a friendly message.
        </li>
        <li>
            <b>"Add Task"</b> Entering a To-Do task within text input and clicking "Add Task" should add the task to the list of To-Do tasks. Duplicate tasks with same text are allowed.
        </li>
        <li>
          <b>"Validate Task"</b> If "Add Task" is clicked without entering any text an Alert or Error containing "Please enter Task" should be displayed.
        </li>
        <li>
          <b>"Mark Task"</b>  Clicking the checkbox next to the task should apply "strikethrough" for the Task text and increase the 'Done' counter.
        </li>
        <li>
          <b>"Remove Task"</b> Clicking the close button of the tasks within the list should delete/it from the list and decrease the 'Done' counter.
        </li>
        <li>
          <b>"Extra Credit"</b> Make the CSS designs responsive and display layout correctly on mobile or tablet or desktop mode.
        </li>
      </ol>



      </div>
  </div>
</template>

<script>
export default {
  name: 'TaskManager',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.task-manager{
  max-width: 700px;
  margin: 0 auto;
}

h3 {
  margin: 40px 0 0;
}

a {
  color: #42b983;
}
img{
  width: 100%;
  height: auto;
}

.task-body ol{
  list-style-type: decimal;
  text-align: left;
  font-size: 14px;
}

.task-body li{
  margin-bottom: 15px;
}

</style>
