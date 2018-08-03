#title{
  
}
body{
  text-align: center;
  background-color: skyblue;
  font-family: Helvetica, sans-serif;
}
.main-form{
  background-color: white;
  border-radius: 4px;
  max-width: 900px;
  margin: 0 auto;
  padding-top: 20px;
}
#survey-form{}
#description{
  color: green;
  padding-top: 15px
}
#name{
  height: 20px;
  
  padding: 5px;
  margin: 10px;
  border: 1px solid #c0c0c0;
  border-radius: 2px;
}
#email{
  height: 20px;
  
  padding: 5px;
  margin: 10px;
  border: 1px solid #c0c0c0;
  border-radius: 2px;
}
#name-label{
  display: inline-block;
  text-align: right;
  width: 40%;
  padding: 5px;
  vertical-align: top;
  margin-top: 10px;
}
#number{
  height: 20px;
  padding: 5px;
  margin: 10px;
  border: 1px solid #c0c0c0;
  border-radius: 2px;
}
#email-label{
  display: inline-block;
  text-align: right;
  width: 40%;
  padding: 5px;
  vertical-align: top;
  margin-top: 10px;
}
#number-label{
  display: inline-block;
  text-align: right;
  width: 40%;
  padding: 5px;
  vertical-align: top;
  margin-top: 10px;
}
#dropdown {
  height: 35px;
  width: 140px;
  padding: 5px;
  margin: 10px;  
  margin-top: 15px;
  border: 1px solid #c0c0c0;
  border-radius: 2px;
}
.radio, .checkbox {
  position: relative;
  left: -43px;
  
  margin-left: 10px;
  display: block;
  padding-bottom: 10px;
}
#comments{
  box-align: left;
}
#submit {
  background-color: #59ace0;
  border-radius: 4px;
  color: white;
  font-size: 1em;
  height: 40px;
  width: 96px;
  margin: 10px;
  border: 0px solid;
}

<h1 id="title">Survey form</h1>
<div>
  <form id="survey-form" class="main-form">
    <p id="description">This is the survey form to rate my projects</p>
    <div>
      <label id="name-label">*Name: <input id="name" type="text" placeholder="Enter your name"required></label><br>
      <label id="email-label">*Email: <input id="email" type="email" name="email" placeholder="Please enter your email" required></label><br>
      <label id="number-label">*Age<input id="number" type="number" min="18" max="60" name="age" placeholder="Age"></label>
    </div>
    <div>
      <label for="currentPos">Please advise:</label>
      <select id="dropdown">
        <option disabled value> Choose option</option>
        <option value> Style</option>
        <option value name="content"> Content</option>
      </select>
    </div>
    <div>
      <label>How likely could you refer me to a friend</label>
      <div> 
        <ul style="list-style: none;">
          <li class="radio"> <label>Yes<input type="radio" value="1" name="radio-buttons"></label>
            </li>
          <li class="radio">
            <label>No <input type="radio" value="2" name="radio-buttons"></label>
          </li>
        </ul>
      </div>
    </div>
    <div>
      <label for="currentPos">Things that should be improved:</label>
      <div>
        <ul class="checkbox" style="list-style: none;">
          <li><label>Front-end <input type="checkbox" value="1"></label></li>
          <li>
            <label>Back-end <input type="checkbox" value="2"></label>
          </li>
          <li><label>Data Visualisation <input type="checkbox" value="3"></label></li>
        </ul>
      </div>
    </div>
    <div>  
      <div>
        <label for="comment">Comments:</label>
      </div>
      <textarea id="comments" placeholder="enter your comment"></textarea>
    </div>
    <button id="submit" type="submit">Submit</button>
  </form>
</div>
