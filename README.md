Marty: if you get the chance can you exmplain the changes you made to the database? I'm a little confused about why question and answers need a join table. The database refactoring means we have to remake all the other pgaes that rely on it, and to do that, I need to understand what's going on there.

You think you'll make it in tomorrow?


Cool deal, martin, thanks. I was just trying to get a better grasp on the context of whatever problem you were having.

Hing and I are having fun implementing cool things. Have a great night; we'll see you later.

i will try and look at them tonight.  What the results page is trying to accomplish is to display each answer along with the number of times the answer has been picked by all users.  Im in the middle of a whirlwind of children and noise and am not thinking straight, will continue working tomorrow though to implement a javascript bar graph.



when you have time martin check out the new index and create survey page.

 celeen: did you figure this out? why are we trying to count a single answer id? What is this code trying to accomplish? What errors are you getting? wat?

 need some help with line 10 in the survey_result erb.

                <li><%=question.content%> = <%=QuestionAnswers.where(question_id: question.id, answer_id: answer.id.count %></li>


Sounds Good. GO FOR IT. =)



this is the code I am going to try and use to do the graph I think.  I am going to have to add another model/migration table. We will need a questions/answer join table that will keep track of what awnsers are chosen for what questions, I think printing results would otherwise be impossible.  What do you guys think?

i made the route and a simple display for it, but have not employed it yet.





