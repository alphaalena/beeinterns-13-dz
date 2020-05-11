<template>
  <form class="form">
    <text-component>Review before the test (check if done)</text-component>
    <row-component>
      <column-component>
        <row-component justify-start>
          <input type="checkbox" id="checkbox" class="checkbox">
          <label for="checkbox">Email Participants</label>
        </row-component>
        <text-component little class="indent">If checked, write the date that was sent</text-component>
        <text-component little-fatty class="indent">Date:</text-component>
      </column-component>
      <column-component>
        <text-component>Reminder participants about the tests</text-component>
        <text-component little class="indent">Write the number and dates of the<br>reminders<br>
          If reminder was done, please check the box
        </text-component>
        <row-component justify-start class="indent">
          <input type="checkbox" id="checkbox1" class="checkbox">
          <label for="checkbox1" style="font-weight: bold">Reminder #1 - Date:</label>
        </row-component>
        <row-component justify-start class="indent">
          <input type="checkbox" id="checkbox2" class="checkbox">
          <label for="checkbox2" style="font-weight: bold;">Reminder #2 - Date:</label>
        </row-component>
      </column-component>
      <column-component justify-content>
        <row-component justify-start>
          <input type="checkbox" id="first" class="checkbox">
          <label for="first">Ethical Approval prepared and sent</label>
        </row-component>
        <row-component justify-start>
          <input type="checkbox" id="second" class="checkbox">
          <label for="second">Recording consent
            prepared for the test session</label>
        </row-component>
        <row-component justify-start>
          <input type="checkbox" id="third" class="checkbox">
          <label for="third">Usability testing checklist prepared for the test session</label>
        </row-component>
      </column-component>
    </row-component>
  </form>
</template>
<script>
import TextComponent from './text-component'
import RowComponent from './row-component'
import ColumnComponent from './column-component'

export default {
  name: 'ReviewComponent',
  components: {
    ColumnComponent,
    RowComponent,
    TextComponent
  }
}
</script>
<style>
  .form {
    width: 850px;
    height: 197px;
    background: #F6F9FF;
    border-radius: 8px;
    text-align: left;
    padding: 8px 44px 8px 8px;
  }
  .checkbox {
    margin-right: 6px;
  }
  .indent {
    margin-left: 30px;
  }
</style>
