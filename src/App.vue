<template>
  <div id="app">
    <row-component justify-start>
      <column-component>
        <usability-test-component>
          <heading-component>usability test plan dashboard</heading-component>
          <text-component>The sercive/product that is going to be tested</text-component>
          <section-columns-component/>
          <text-component>Business requirements</text-component>
          <section-columns-component/>
          <text-component>User requirements</text-component>
          <section-columns-component/>
          <text-component>Location & dates of the tests</text-component>
          <section-columns-component/>
        </usability-test-component>
      </column-component>
      <column-component class="color">
        <text-component>Test Objectives</text-component>
        <row-component justify-start>
          <test-objectives-component>
            <text-component text-opacity>Why are you doing this user testing? What are the benefits Any risks of not
              achieving this test?
            </text-component>
          </test-objectives-component>
          <test-objectives-component>
            <text-component text-opacity>
              What are the goals of the usabilty test? What are the specific questions that
              will be answered? What hypothesis that will be tested?
            </text-component>
          </test-objectives-component>
        </row-component>
        <text-component>Test Preparation</text-component>
        <row-component>
          <preparation-component>
            <row-component justify-start>
              <column-component>
                <row-component justify-start>
                  <responsibility-component>
                    <text-component>
                      Teams who are involved and what are their responsibilities?
                    </text-component>
                  </responsibility-component>
                  <test-plan-component>
                    <text-component>
                      Test plan / procedure
                    </text-component>
                    <text-component text-opacity>
                      List the main steps of the test procedure
                    </text-component>
                    <row-component justify-start>
                    <block-component :key="number" v-for="number in numbers">{{number}}</block-component>
                    </row-component>
                  </test-plan-component>
                </row-component>
                <review-component/>
              </column-component>
              <test-tasks-component>
                <text-component>Test Tasks</text-component>
                <text-component text-opacity>List the test tasks</text-component>
              </test-tasks-component>
            </row-component>
          </preparation-component>
        </row-component>
      </column-component>
    </row-component>

  </div>
</template>

<script>
import ColumnComponent from './components/column-component'
import RowComponent from './components/row-component'
import UsabilityTestComponent from './components/Usability-test-component'
import HeadingComponent from './components/heading-component'
import SectionColumnsComponent from './components/sectionColumns-component'
import TextComponent from './components/text-component'
import TestObjectivesComponent from './components/Test-Objectives-components'
import PreparationComponent from './components/Preparation-component'
import ResponsibilityComponent from './components/responsibility-component'
import TestPlanComponent from './components/test-plan-component'
import ReviewComponent from './components/Review-component'
import TestTasksComponent from './components/test-tasks-component'
import BlockComponent from './components/block-component'

export default {
  name: 'App',
  components: {
    BlockComponent,
    TestTasksComponent,
    ReviewComponent,
    TestPlanComponent,
    ResponsibilityComponent,
    PreparationComponent,
    TestObjectivesComponent,
    UsabilityTestComponent,
    TextComponent,
    SectionColumnsComponent,
    HeadingComponent,
    RowComponent,
    ColumnComponent
  },
  data () {
    return {
      numbers: [1, 2, 3, 4, 5, 6, 'Текста']
    }
  }
}
</script>

<style>
  #app {
    font-family: Arimo sans-serif;
    font-size: 14px;
    line-height: 16px;
    color: #4A4A4A;

  }
</style>
