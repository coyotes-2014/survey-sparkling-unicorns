when you have time martin check out the new index and create survey page.

 celeen: did you figure this out? why are we trying to count a single answer id? What is this code trying to accomplish? What errors are you getting? wat?
 
 need some help with line 10 in the survey_result erb.

                <li><%=question.content%> = <%=QuestionAnswers.where(question_id: question.id, answer_id: answer.id.count %></li>


Sounds Good. GO FOR IT. =)



this is the code I am going to try and use to do the graph I think.  I am going to have to add another model/migration table. We will need a questions/answer join table that will keep track of what awnsers are chosen for what questions, I think printing results would otherwise be impossible.  What do you guys think?

i made the route and a simple display for it, but have not employed it yet.




 	<script type="text/javascript">
 		$(function () {
     	$('#container').highcharts({

         chart: {
             type: 'column',
             options3d: {
                 enabled: true,
                 alpha: 15,
                 beta: 15,
                 viewDistance: 25,
                 depth: 40
             },
             marginTop: 80,
             marginRight: 40
         },

         title: {
             text: 'Total fruit consumption, grouped by gender'
         },

         xAxis: {
             categories: ['Apples', 'Oranges', 'Pears', 'Grapes', 'Bananas']
         },

         yAxis: {
             allowDecimals: false,
             min: 0,
             title: {
                 text: 'Number of fruits'
             }
         },

         tooltip: {
             headerFormat: '<b>{point.key}</b><br>',
             pointFormat: '<span style="color:{series.color}">\u25CF</span> {series.name}: {point.y} / {point.stackTotal}'
         },

         plotOptions: {
             column: {
                 stacking: 'normal',
                 depth: 40
             }
         },

         series: [{
             name: 'John',
             data: [5, 3, 4, 7, 2],
             stack: 'male'
         }, {
             name: 'Joe',
             data: [3, 4, 4, 2, 5],
             stack: 'male'
         }, {
             name: 'Jane',
             data: [2, 5, 6, 2, 1],
             stack: 'female'
         }, {
             name: 'Janet',
             data: [3, 0, 4, 4, 3],
             stack: 'female'
         }]
     });
 });
    
 	</script>
