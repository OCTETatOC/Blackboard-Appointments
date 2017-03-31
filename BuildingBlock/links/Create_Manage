<bbUI:stepContent>
Make the appointments available<br>
  <label>
  	<input name="courseIDs[]" type="checkbox" value="DIRECTORY">
  	Show in directory tool</label><br>
  <label>
  	<input name="courseIDs[]" type="radio" value="ALL" onchange="checkAll()"> <%--default = checked --%>
  	Available for all courses/organizations</label>.<br>
  <label>
  	<input name="courseIDs[]" type="radio" id="selectCourse" checked onchange="checkAll()">
  	Available in selected courses/organizations</label>.<br>
<%--Will list out the available courses you are an instructor for.--%>
<%--Personal note: using < % and % > gets into javascript coding mode. --%>
<%-- course.getCourseId() gets the id of the course within courses. getTitle() then print the name of the course --%>
<%-- we don't use cId or any of the variables above because they refer to only one course that we're in, not what we have in courses --%>
<%--list all courses if the previous box was checked--%>
<%--part will only appear if above is checked--%>
<div id="courseList" style="visibility: visible; position: relative; left: 25px;">
<% for (Course course: courses){ %>
	<input type="checkbox" name="courseIDs[]" value=<%=course.getCourseId()%>> <%=course.getTitle()%><br>
<% } %>
</div>
