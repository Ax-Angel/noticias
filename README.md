noticias
========
<html>
<head>

  <!-- Google font embed code -->
	<link href=
	'http://fonts.googleapis.com/css?family=Droid+Sans|Roboto+Condensed' rel=
	'stylesheet' type='text/css'>

	<title>&#C1C6EC;Hermes El Mensajero</title>


	<!-- Meta tags are meta -->
	<meta name="description" content="Noticias Mundiales en español">
	<meta name="keywords" content="Noticias, Tecnología, Espectaculo, Política">
	<meta name="author" content="Angel Rodríguez">
	<meta charset="UTF-8">


	<!-- jQuery from Google embed code -->
	<script src=
	"http://ajax.googleapis.com/ajax/libs/jquery/2.0.0/jquery.min.js" type=
	"text/javascript"></script>


	<!-- Stylesheet linker code -->
	<link href="newsbeard.css" rel="stylesheet" type="text/css">
</head>

<body>
	<!-- JSON URL for Yahoo Pipes - http://pipes.yahoo.com/pipes/pipe.run?_id=18622a1798c0dd2b3f54c07f6ed7d489&_render=json
	-->


	<!-- Big orange banner code -->
	<ul class="rss-title">
		<li class="mast" style="float:left"><strong><a href="http://newsbeard.com/" style=
		"text-decoration:none">&#187;Newsbeard<small><sup>beta</sup></small><a></a></strong></li>
		<li class="refresh"  style="float:right"><a href="http://newsbeard.com/refresh.html" style=
		"text-decoration:none">&nbsp;&nbsp;<img src="rec.png" height=24px width=24px> Off&nbsp;</a></li>
	</ul>


	<!-- Div container for article list -->
	<div id="rssdata">
		<ul class="rss-items"></ul>


	<!-- Loading message -->
		<div class="loading">
			<center></strong>&#187;Loading Newsbeard...</center></strong> 


	<!-- jQuery content grabber from Pipes -->
	<script type="text/Javascript">
		$('#rssdata').ready(function()
			{
			var pipe_url = 'http://pipes.yahoo.com/pipes/pipe.run?_id=18622a1798c0dd2b3f54c07f6ed7d489&_render=rss';
			$.getJSON(pipe_url,function(data)
			{
			$(data.value.items).each(function(index,item)
			{
			var item_html = '<li><a href="'+item.link+'">'+item.title+'<\/a><\/li>';
			$('#rssdata ul.rss-items').append(item_html);
			});
			$('#rssdata div.loading').fadeOut();
			$('#rssdata ul.rss-items').slideDown();
			});
			});
			</script>
		</div>
	</div>


	<!-- Google analytics -->
	<!-- Replace this with your own code if you use this -->
	<script>
  	(function(i,s,o,g,r,a,m){i['GoogleAnalyticsObject']=r;i[r]=i[r]||function(){
  	(i[r].q=i[r].q||[]).push(arguments)},i[r].l=1*new Date();a=s.createElement(o),
  	m=s.getElementsByTagName(o)[0];a.async=1;a.src=g;m.parentNode.insertBefore(a,m)
  	})(window,document,'script','//www.google-analytics.com/analytics.js','ga');

  	ga('create', 'UA-40528442-1', 'newsbeard.com');
 	 ga('send', 'pageview');
	</script>




	<!-- Orange footer bar for license or whatever -->
	<ul class="rss-footer">
	<li>	
	<!-- OMG MOBILE ADVERTISING OH SNAP -->
	<script type="text/javascript">
	<!--
	google_ad_client = "ca-pub-3251177579129524";
	/* Newsbeard */
	google_ad_slot = "8195839875";
	google_ad_width = 320;
	google_ad_height = 50;
	//-->
	</script>
	<script type="text/javascript"
	src="http://pagead2.googlesyndication.com/pagead/show_ads.js">
	</script>
	</li></ul>


</body>
</html>
