function customTag(tagName,fn){
  document.createElement(tagName);
  //find all the tags occurrences (instances) in the document
  var tagInstances = document.getElementsByTagName(tagName);
    //for each occurrence run the associated function
        for ( var i = 0; i < tagInstances.length; i++) {
            fn(tagInstances[i]);
        }
}
 
function codingdudeGravatar(element){
        //code for rendering the element goes here
        if (element.attributes.email){
            //get the email address from the element's email attribute
            var email = element.attributes.email.value;
            var gravatar = "http://www.gravatar.com/avatar/"+md5(email)+".png";
            element.innerHTML = "<img src='"+gravatar+"'>";
        }
}   
 
customTag("codingdude-gravatar",codingdudeGravatar);
