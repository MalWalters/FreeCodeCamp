$("#newQuote").on("click", function(){

  $.ajax({
    url: 'https://andruxnet-random-famous-quotes.p.mashape.com/?cat=movies', 
    type: 'GET', 
    data: {}, 
    datatype: 'json',
    success: function(data) { 
      //var jsonData = JSON.stringify(data);
      var jsonData = Object.keys(data);
      
      jsonData.forEach(function(key) {
        $(".quote").html(data[key]);               
                       });
  
      //$(".quote").html(jsonData);
      //$(".author").html("Bye.");
      //Change this to update the quote area
      //Split the data up into quote and author section.
      //alert(JSON.stringify(data));
    },
    error: function(err) { alert(err); },
    beforeSend: function(xhr) {
    xhr.setRequestHeader("X-Mashape-Authorization", "4IDmirmdNKmshjl1h2g5hR9zk3cIp1Q2aOwjsnZUoXxIZhDOYc"); 
    }
});
})
