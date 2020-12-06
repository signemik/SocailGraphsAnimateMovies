<!--<!DOCTYPE html>-->
<html lang="en">

<!--<head>-->

<!-- title and meta -->
<meta charset="utf-8" />
<meta name="viewport" content="width=device-width,initial-scale=1.0" />
<meta name="description" content="" />

<title> Animated Movies |  Social Graphs 2020</title>

<!-- css -->
<link href='https://fonts.googleapis.com/css?family=Ubuntu:300,400,700,400italic' rel='stylesheet' type='text/css'>
<link href='https://fonts.googleapis.com/css?family=Oswald:400,300,700' rel='stylesheet' type='text/css'>
<link rel="stylesheet" href="css/style.css" />
<!--<link rel="stylesheet" href="css/twitter-quotes.css">-->
<link rel="stylesheet" href="css/switch.css" />
<link rel="stylesheet" type="text/css" href="css/slick.css"/>
<link rel="stylesheet" type="text/css" href="css/slick-theme.css"/>
<link rel="stylesheet" type="text/css" href="css/bar.css"/>

<!-- js -->
<script src="js/classie.js"></script>
<script src="js/jquery-3.1.1.min.js"></script>
<script src="js/scroll.js"></script>
<script src="js/parallaxImg.js" type="text/javascript"></script>
<script src="js/parallaxImg.js"></script>
<script src="js/quotes.js"></script>
<script src="js/select.js"></script>
<script src="js/masonry.pkgd.min.js"></script>
<script src="js/jquery.flexslider-min.js"></script>
<script src="nodes_modules/d3/build/d3.min.js"></script>
<script src="nodes_modules/d3-tip/index.js"></script>
<script src="js/jquery.js" type="text/javascript"></script>
<meta name="viewport" content="width=device-width, initial-scale=1">
<link rel="stylesheet" href="https://www.w3schools.com/w3css/4/w3.css">
<style>
.mySlides {display:none}
</style>
<body>

<div class="w3-container">
  <h2>Slideshow Indicators</h2>
  <p>An example of using buttons to indicate how many slides there are in the slideshow, and which slide the user is currently viewing.</p>
</div>


<div class="w3-content" style="max-width:800px">
  <p align="center">
  <img class="mySlides" src="Images/sentiment-analysis.jpg" style="width:20%">
  <img class="mySlides" src="Images/sentiment-analysis.jpg" style="width:20%">
  <img class="mySlides" src="Images/network-analysis.jpg" style="width:20%">
  </p>
</div>
<div class="w3-center">
  <div class="w3-section">
    <button class="w3-button w3-light-grey" onclick="plusDivs(-1)">❮ Prev</button>
    <button class="w3-button w3-light-grey" onclick="plusDivs(1)">Next ❯</button>
  </div>
  <button class="w3-button demo" onclick="currentDiv(1)">1</button> 
  <button class="w3-button demo" onclick="currentDiv(2)">2</button> 
  <button class="w3-button demo" onclick="currentDiv(3)">3</button> 
</div>

<script>
 var slideIndex = 1;
showDivs(slideIndex);

function plusDivs(n) {
  showDivs(slideIndex += n);
}

function currentDiv(n) {
  showDivs(slideIndex = n);
}

function showDivs(n) {
  var i;
  var x = document.getElementsByClassName("mySlides");
  var dots = document.getElementsByClassName("demo");
  if (n > x.length) {slideIndex = 1}
  if (n < 1) {slideIndex = x.length}
  for (i = 0; i < x.length; i++) {
    x[i].style.display = "none";  
  }
  for (i = 0; i < dots.length; i++) {
    dots[i].className = dots[i].className.replace(" w3-white", "");
  }
  x[slideIndex-1].style.display = "block";  
  dots[slideIndex-1].className += " w3-white";
}
</script>
</body>


<!--<script src="js/jquery.nicescroll.min.js" type="text/javascript"></script>
<script src="js/parallaxImg.js" type="text/javascript"></script>
 <link rel="stylesheet" type="text/css" href="css/demotheme.css">
  <meta name="viewport" content="width=device-width, initial-scale=1, user-scalable=no">
  <script type="text/javascript">
    $(document).on("ready", function() {
      var parallaxSettings = {
        initialOpacity: 1, //from 0 to 1, e.g. 0.34 is a valid value. 0 = transparent, 1 = Opaque
        opacitySpeed: 0.1, //values from 0.01 to 1 -> 0.01: slowly appears on screen; 1: appears as soon as the user scrolls 1px
        pageLoader: true
      };

      parallaxImgScroll(parallaxSettings);
    });-->
<!-- </header>/header -->



<div id="main" class="first_main">
    <div id="content">
        <section id="one">
            <div class="container">
                <h1 id="contenttitle">Contents</h1>

                <p align="center"> <!--<class="contents">-->
                    <a href="#network"><img height="150" src="Images/network-analysis.jpg"><br>
                    &rarr; Network Analysis</a><br><br>
                    <a href="#sentiments"><img height="150" src="Images/sentiment-analysis.jpg"><br>
                    &rarr; Sentiment Analysis</a><br><br>
                </p>
            </div>
             </section>
        <section class="color" id="network">
            <div class="container">
                <h1>Network analysis </h1>
                <div class="w3-content w3-display-container">
                  <img class="mySlides" src="Images/sentiment-analysis.jpg">
                  <img class="mySlides" src="Images/sentiment-analysis.jpg">
                  <img class="mySlides" src="Images/sentiment-analysis.jpg">
                  <div class="w3-center w3-display-bottommiddle" style="width:100%">
                   <div class="w3-left" onclick="plusDivs(-1)">&#10094;</div>
                    <div class="w3-right" onclick="plusDivs(1)">&#10095;</div>
                    <span class="w3-badge demo w3-border" onclick="currentDiv(1)"></span>
                    <span class="w3-badge demo w3-border" onclick="currentDiv(2)"></span>
                    <span class="w3-badge demo w3-border" onclick="currentDiv(3)"></span>
                   </div>
                  </div>
                  </div>
                
                
                <br>
                <p>
                  Politicians is heavy users of twitter and the retweet functionality is often used to share the tweets from other politicians.
                  But how are these retweets connected? Do politician tend to retweet each other more within the same party? Can a party be detected by using the Louvain
                  algorithm to detect communities?
                </p>
                <p>
                  When politicians talk in the parliament they often mention each other in different contexts whether they agree or disagree with each other.
                  How are these politicians connected when it comes to mentioning each other? Are some politicians central for the parliament? do politicians within the same
                  party mention each other more often than politicians from other parties?
                </p>
                <div>
                  <svg id="svg-graph" width="800" height="600" style="float:left"></svg>
                  <div style="margin: 0 auto; width: 400px; overflow:hidden; height:600px">
                    <div style="width:250px; display:block">
                      <p style="float:left">Community</p>
                      <label class="switch" style="margin-left: 60px">
                        <input id="comBox" type="checkbox" onchange="toggleCheckbox(this)">
                        <div class="slider round" style="background-color:#ccc"></div>
                      </label>
                      <p style="float:right;margin-right: -8px;">Party</p>
                    </div>
                    <div style="width:400px; display:block;">
                      <p style="margin-left:-82px; float:left">Retweet network</p>
                      <label class="switch" style="margin-left: 20px">
                        <input type="checkbox" onchange="changeNetwork(this)">
                        <div class="slider round"style="background-color:#ccc"></div>
                      </label>
                      <p style="float:right; margin-right:40px">Parliament meeting</p>
                    </div>
                    <div style="width:250px; height:50px">
                      <p style="margin-left: -125px;margin-top:20px;float:left;">Node size</p>

                      <div class="dropdown" style="width:160px">
                        <button onclick="myFunction()" id="dropbtn" class="dropbtn">Static</button>
                        <div id="myDropdown" class="dropdown-content">
                          <a onclick="nodeSize('Static')">Static</a>
                          <a onclick="nodeSize('In degree')">In degree</a>
                          <a onclick="nodeSize('Out degree')">Out degree</a>
                          <a onclick="nodeSize('Betweenes centrality')">Betweenness centrality</a>
                          <a onclick="nodeSize('In degree eigenvector centrality')">In degree eigenvector centrality</a>
                          <a onclick="nodeSize('Out degree eignevector centrality')">Out degree eignevector centrality</a>
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
                <p>
                  The Louvain algorithm does seem to detect 5 different communities, some more distinct than others. This leads us to the previously asked question; do politicians from
                  the same party tend to retween each other more often and therefore shows the parties as communities in the graph? Coloring the politician nodes with the color
                  representing their party indicates that the algorithm quiet succesfully managed to find the parties as communities meaning that the politicians do tend to retweet
                  more within their own party.<br>
                  Another thing to notice is that both the in and out degree eigenvector centrality is dominant in Socialdemokratiet meaning they often retweet tweets from
                  politicians that often retweet others and that they often get retweeted by politicians that retweet alot of other politicians. The fact that it appears for both the
                  in and the out degree eigenvector centrality implies that the politicians in Socialdemokratiet retweet alot and mostly within their own party.
                </p>
                <p>
                  Switching to the parliament graph reveals a new much bigger graph with the three communities found by the Louvain algorithm represented by colors.
                  The communities does not seem to be very distinct as they all cluster in one big group. Coloring the politician nodes with color based on their party does not
                  indicate a connection between politicians from the same party. This means that politicians do not mention each other more often within the same party but rather
                  mentions other politicians more stochastic.<br>
                  Looking at the betweenness centrality shows that a few politicians seem to dominate the shortest paths, namely Per Clausen from Enhedslisten seem to have a high
                  betweenness centrality.<br>
                  Another interesting thing to notice is the out degree eigenvector centrality for Mogen Lykketoft from Socialdemokratiet. It is extremely high compared to other
                  politicians meaning that he is mentioning alot of politician who also mention alot of other politicians.
                </p>
            </div>
        </section>
    </div>
    
    <div class="parallax-img-container"></div>
        <section class="container" id="terms">
            <div class="container"><br><br>
                <h1>What are the important terms in politics?</h1>
                <p>Let's have a look at the most important terms in Danish politics throughout the last years.</p>

                <h2>The most important words on <b>Twitter</b> (2009-2016)</h2><br>
                <div class="cloud-car">
                    <div class="single-item">
                        <img src="Images/sentiment-analysis.jpg" alt="">
                        <p>Twitter TF-IDF 03-2009 - 06-2009</p>
                    </div>
                    <div class="single-item">
                        <img src="Images/sentiment-analysis.jpg" alt="">
                        <p>Twitter TF-IDF 06-2009 - 09-2009</p>
                    </div>
                    <div class="single-item">
                        <img src="Images/sentiment-analysis.jpg" alt="">
                        <p>Twitter TF-IDF 09-2009 - 12-2009</p>
                    </div>
                    <div class="single-item">
                        <img src="Images/sentiment-analysis.jpg" alt="">
                        <p>Twitter TF-IDF 12-2009 - 03-2010</p>
                    </div>
                    <div class="single-item">
                        <img src="Images/sentiment-analysis.jpg" alt="">
                        <p>Twitter TF-IDF 03-2010 - 06-2010</p>
                    </div>
                    <div class="single-item">
                        <img src="Images/sentiment-analysis.jpg" alt="">
                        <p>Twitter TF-IDF 06-2010 - 09-2010</p>
                    </div>
                    <div class="single-item">
                        <img src="Images/sentiment-analysis.jpg" alt="">
                        <p>Twitter TF-IDF 09-2010 - 12-2010</p>
                    </div>
                    <div class="single-item">
                        <img src="Images/sentiment-analysis.jpg" alt="">
                        <p>Twitter TF-IDF 12-2010 - 03-2011</p>
                    </div>
                    <div class="single-item">
                        <img src="Images/sentiment-analysis.jpg" alt="">
                        <p>Twitter TF-IDF 03-2011 - 06-2011</p>
                    </div>
                    <div class="single-item">
                        <img src="Images/sentiment-analysis.jpg" alt="">
                        <p>Twitter TF-IDF 06-2011 - 09-2011</p>
                    </div>
                </div>
                <br>

                <p>Notice that quite a lot of important events can be identified in the important terms from the tweets. Some examples would be:
                <ul>
                    <li>
                        <p>     - Conflicts &amp; Wars (e.g. Libya, Ukraine)</p>
                    </li>
                    <li>
                        <p>     - Elections (KV, FV, EU)</p>
                    </li>
                    <li>
                        <p>     - Scandals (e.g. tax havens, information hiding, etc.)</p>
                    </li>
                </ul></p>

                <h2>How about in the <b>parliament</b>? (2010-2016)</h2>
                <p>Similarly, we can look at the most important terms from the meetings within the Danish parliament throughout the last years.</p>

                <p>The important terms extracted from the Danish parliament seem to confirm the notion that real politics is a boring business. Jokes aside, the wordclouds does seem to represent a less colorful corpus of words. This makes sense intuitively, as Twitter is (or was) limited to 140 characters, which forces its messenger to create a strong, clear, and to-the-point wording, while meetings in the parliament can go on for hours.</p>
                <p>Looking at the most weighted terms (rare words) across all documents does seem to capture some of the colors that frequent terms has washed out:</p>

                <img src="img/wordcloud-all.png" alt="" id="cloudplot">

                <h2>Clustering by important terms</h2>
                <p>Usinger sklearn's linear kernel module, we can compute the pairwise cosine similarity between politicians and parties. After the similarities have been determined, we can cluster the politicians or parties, using our favourite clustering algorithm. We tried spectral clustering and KMeans that worked quite well for this particular task.</p>

                <div class="twoplotc"><img src="img/party_2_plots.png" alt="" class="twoplots" id="cloudplot"><img src="img/party_3_plots_spectral.png" alt="" class="twoplots" id="cloudplot"></div>

                <p>From the plots we can see that when we set the clustering method two extract two plots, the Danish parties are creating one cluster while the foreign parties (Faroe Islands and Greenland) are creating another.</p>
                <p>For three clusters we see that Alternativet, Kristendemokraterne and Non-Party Members join in on a new cluster.</p><br><br>

            </div>
        </section>
        </section>
    </div>
</div><!-- #main -->
        </section>
        <section class="color" id="sentiments">
            <div class="container">
                <h1>Sentiemnt analysis</h1>
                <p>Emotions are everywhere. Especially in politics.<br>
                Recently, The Oxford Dictionaries announced that its Word of the Year 2016 is <b>post-truth</b>.<br>
                </p>
                <img src="img/woty.png" id="woty">

                <blockquote><p>‘relating to or denoting circumstances in which objective facts are less influential <br>in shaping public opinion than appeals to emotion and personal belief’</p>
                <br><span>- 'Post-truth' according to The Oxford Dictionaries</span></blockquote>
                <p>The frequent use of a word such as 'post-truth' indicates that people seem to think that politics are increasingly
                  prefering emotions to fact. Pathos to logos. But is this true? We investigated how emotions are showing in the
                  Danish parliament and on Danish politicians' Twitter feeds. The Danish parliament dataset was extracted using web scraping from transcipted parliament meetings and
                  the twitter dataset was generated using the twitter API and contains tweets from 149 Danish politicians.</p>

                <h2>Emotions over time</h2>
                <p>Let's get an overview of the emotional spectrum by looking at the weekly average of emotions on Danish politicians' Twitter and in the parliament:</p>

                <img src="img/plots/sent-time.png" class="plot">
                <p>The graphs seem to be quite well correlated. It should be noted that the method of calculating the sentiments was to add up positive and negative sentiment values of each word in a text. Averaging the blocks of text makes it more likely for longer text blocks to have extreme values (positive or negative), which is probably why the sentiment of the parliament is generally higher than on twitter.</p>

                <h1>How are politicians sentiment in the parliament compared to their twitter sentiment?</h1>
                <p>
                  We sometimes experience that people behave different in real life compared to their online behaviour. Examining the sentiment of tweets from danish politicians
                  and comparing it to the sentiment of when they are talking in the parliament meetings shows the average and standard deviation of each politicians sentiment both on
                  twitter and in the meetings. A high average sentiment and low standard deviation sentiment implies a high sentiment in general while a high standard deviation implies
                  a high level of expressivenes.
                <br>
                Top 3 positive tweets:</p>

                <div class="cd-testimonials-wrapper cd-container positive">
                    <ul class="cd-testimonials">
                        <li>
                            <p>I dag er det DFs fødselsdag hurra hurra hurra
                            Vi sikkert mange gaver får
                            Som vi har ønsket os i år
                            For 21 år er vel en gave værd
                            #dkpol</p>
                            <div class="cd-author">
                                <img src="img/Morten_Marinus.jpg" alt="Morten Marinus">
                                <ul class="cd-author-info">
                                    <li>Morten Marinus</li>
                                    <li>DF</li>
                                </ul>
                                <span class="cd-number">1.</span>
                            </div>
                        </li>

                        <li>
                            <p>"Messerschmidt har aldrig sat sig ind i, hvordan EU fungerer..." (citat Anna Rosbach i Berlingske). Ha-ha-ha-ha-ha-ha-ha-ha-ha-ha..! #dkpol</p>
                            <div class="cd-author">
                                <img src="img/Soeren_Espersen.jpg" alt="Søren Espersen">
                                <ul class="cd-author-info">
                                    <li>Søren Espersen</li>
                                    <li>DF</li>
                                    <span class="cd-number">2.</span>
                                </ul>
                            </div>
                        </li>

                        <li>
                            <p>Hej @FradragNu - Det er mig der takker for super god inspiration til iværksætterpolitik hos @Spolitik - held og lykke med fradrag.nu #dkpol</p>
                            <div class="cd-author">
                                <img src="img/Thomas_Jensen.jpg" alt="Thomas Jensen">
                                <ul class="cd-author-info">
                                    <li>Thomas Jensen</li>
                                    <li>Socialdemokraterne</li>
                                    <span class="cd-number">3.</span>
                                </ul>
                            </div>
                        </li>

                    </ul> <!-- cd-testimonials -->

                    <a href="#0" class="cd-see-all">See all</a>
                </div> <!-- cd-testimonials-wrapper -->

                <h2>DF seems to be the happiest party on Twitter, but...</h2>
                <p>Søren Espersen's tweet that is ranked as the second happiest in our records is a great example of a quirk when calculating sentiments using a list of labelled words.<br>
                When reading the tweet as a human, it is obvious that the tweet is sarcastic and not very positive. However, being limited to look at each word, our algorithm count the long string of Ha-ha-ha... as very positive. <br>
                Now, let's have a look at the top 3 negative tweets:</p>

                <div class="cd-testimonials-wrapper cd-container negative">
                    <ul class="cd-testimonials">
                        <li>
                            <p>Fuck fuck fuck Andrew er ikke videre. Øv!!! En voksen mand m rock under vesten - og så kunne han synge. Fuck! #xfactordr</p>
                            <div class="cd-author">
                                <img src="img/pia-olsen.jpg" alt="Pia Olsen Dyhr">
                                <ul class="cd-author-info">
                                    <li>Pia Olsen Dyhr</li>
                                    <li>SF</li>
                                </ul>
                                <span class="cd-number">1.</span>
                            </div>
                        </li>

                        <li>
                            <p>WTF? @sorenpind kobler skærpet straf for voldtægt og skærpet straf for falsk anklage #usagligt #sexisme #dkpol https://t.co/eNbeEtoH5x</p>
                            <div class="cd-author">
                                <img src="img/pernille-skipper.jpg" alt="Pernille Skipper">
                                <ul class="cd-author-info">
                                    <li>Pernille Skipper</li>
                                    <li>Enhedslisten</li>
                                    <span class="cd-number">2.</span>
                                </ul>
                            </div>
                        </li>

                        <li>
                            <p>@ElisabethMJ @Kvindemuseet @finanslov øv, øv, øv, øv og sgu altså. Helt forkert. @rasmusnordqvist har du set det her?</p>
                            <div class="cd-author">
                                <img src="img/uffe.jpg" alt="Uffe Elbæk">
                                <ul class="cd-author-info">
                                    <li>Uffe Elbæk</li>
                                    <li>Alternativet</li>
                                    <span class="cd-number">3.</span>
                                </ul>
                            </div>
                        </li>

                    </ul> <!-- cd-testimonials -->

                    <a href="#0" class="cd-see-all">See all</a>
                </div> <!-- cd-testimonials-wrapper -->

                <p>The most negative tweets ranges from angry, to sad, to ... X-Factor.<br>
                One interesting observation is the distribution of positive/negative politicians based on their party. The top positive tweets mostly include right-wing politicians, while the top negative tweets only include left-wing politicians.</p>

                <div class="cd-testimonials-all">
                    <div class="cd-testimonials-all-wrapper">
                        <ul>
                            <li class="cd-testimonials-item">
                            <p>I dag er det DFs fødselsdag hurra hurra hurra
                            Vi sikkert mange gaver får
                            Som vi har ønsket os i år
                            For 21 år er vel en gave værd
                            #dkpol</p>
                            <div class="cd-author">
                                <img src="img/Morten_Marinus.jpg" alt="Morten Marinus">
                                <ul class="cd-author-info">
                                    <li>Morten Marinus</li>
                                    <li>DF</li>
                                </ul>
                            </div>
                        </li>

                        <li class="cd-testimonials-item">
                            <p>"Messerschmidt har aldrig sat sig ind i, hvordan EU fungerer..." (citat Anna Rosbach i Berlingske). Ha-ha-ha-ha-ha-ha-ha-ha-ha-ha..! #dkpol</p>
                            <div class="cd-author">
                                <img src="img/Soeren_Espersen.jpg" alt="Søren Espersen">
                                <ul class="cd-author-info">
                                    <li>Søren Espersen</li>
                                    <li>DF</li>
                                </ul>
                            </div>
                        </li>

                        <li class="cd-testimonials-item">
                            <p>Hej @FradragNu - Det er mig der takker for super god inspiration til iværksætterpolitik hos @Spolitik - held og lykke med fradrag.nu #dkpol</p>
                            <div class="cd-author">
                                <img src="img/Thomas_Jensen.jpg" alt="Thomas Jensen">
                                <ul class="cd-author-info">
                                    <li>Thomas Jensen</li>
                                    <li>Socialdemokraterne</li>
                                </ul>
                            </div>
                        </li>

                        <li class="cd-testimonials-item">
                            <p>@KlausKblog Fantastisk! Super godt gået!! Jeg bliver glad i låget over folk som os.. haha :-)</p>
                            <div class="cd-author">
                                <img src="img/Laura_Lindahl.jpg" alt="Laura Lindahl">
                                <ul class="cd-author-info">
                                    <li>Laura Lindahl</li>
                                    <li>LA</li>
                                </ul>
                            </div>
                        </li>

                        <li class="cd-testimonials-item">
                            <p>Jeg var enig med HTS i denne del: "Danmark længe leve! Hurra, hurra, hurra!" #ftlive #dkpol</p>
                            <div class="cd-author">
                                <img src="img/Merete_Riisager.jpg" alt="Merete Riisager">
                                <ul class="cd-author-info">
                                    <li>Merete Riisager</li>
                                    <li>LA</li>
                                </ul>
                            </div>
                        </li>

                        <li class="cd-testimonials-item negative">
                            <p>Fuck fuck fuck Andrew er ikke videre. Øv!!! En voksen mand m rock under vesten - og så kunne han synge. Fuck! #xfactordr</p>
                            <div class="cd-author">
                                <img src="img/pia-olsen.jpg" alt="Pia Olsen Dyhr">
                                <ul class="cd-author-info">
                                    <li>Pia Olsen Dyhr</li>
                                    <li>SF</li>
                                </ul>
                            </div>
                        </li>

                        <li class="cd-testimonials-item negative">
                            <p>WTF? @sorenpind kobler skærpet straf for voldtægt og skærpet straf for falsk anklage #usagligt #sexisme #dkpol https://t.co/eNbeEtoH5x</p>
                            <div class="cd-author">
                                <img src="img/pernille-skipper.jpg" alt="Pernille Skipper">
                                <ul class="cd-author-info">
                                    <li>Pernille Skipper</li>
                                    <li>Enhedslisten</li>
                                </ul>
                            </div>
                        </li>

                        <li class="cd-testimonials-item negative">
                            <p>@ElisabethMJ @Kvindemuseet @finanslov øv, øv, øv, øv og sgu altså. Helt forkert. @rasmusnordqvist har du set det her?</p>
                            <div class="cd-author">
                                <img src="img/uffe.jpg" alt="Uffe Elbæk">
                                <ul class="cd-author-info">
                                    <li>Uffe Elbæk</li>
                                    <li>Alternativet</li>
                                </ul>
                            </div>
                        </li>

                        <li class="cd-testimonials-item negative">
                            <p>Frygtelige nyheder fra Paris- igen. Al den vold, terror og drab på uskyldige  mennesker. Tragisk.</p>
                            <div class="cd-author">
                                <img src="img/Jonas_Dahl.jpg" alt="Jonas Dahl">
                                <ul class="cd-author-info">
                                    <li>Jonas Dahl</li>
                                    <li>SF</li>
                                </ul>
                            </div>
                        </li>

                        <li class="cd-testimonials-item negative">
                            <p>Voldtægt er aldrig din skyld. Offer skal ikke efterlades med skam og angst for ikke at blive taget alvorligt #dkpol https://t.co/9OgTSdqe08</p>
                            <div class="cd-author">
                                <img src="img/Trine_Torp.jpg" alt="Trine Schøning Torp">
                                <ul class="cd-author-info">
                                    <li>Trine Schøning Torp</li>
                                    <li>SF</li>
                                </ul>
                            </div>
                        </li>
                        </ul>
                    </div>  <!-- cd-testimonials-all-wrapper -->

            </div>
        </section>
        </section>
    </div>
</div><!-- #main -->
<div class="parallaxPol"></div>

<div id="main">
    <div id="content">
        <section> 
        <div class="container">
                <h1>How about the use of #hashtags on Twitter?</h1>
                <p>The use of hashtags is an effective way to create, emphasize, or send a message.<br>
                How do the use of hashtags differ across the political spectrum? Let's have a look at some stats.<br></p>
                <h2>The most #hashtagging politicians and party</h2>
                <div class="plot-car">
                    <div class="single-item">
                        <img src="Images/sentiment-analysis.jpg" alt="">
                        <p>Most frequently used hashtags by Danish politicians</p>
                    </div>
                    <div class="single-item">
                        <img src="Images/sentiment-analysis.jpg" alt="">
                        <p>Most hashtagging Danish politicians</p>
                    </div>
                    <div class="single-item">
                        <img src="Images/sentiment-analysis.jpg"alt="">
                        <p>Most hashtagging Danish politic party</p>
                    </div>
                </div>
                <br>

                <p>Notice that #dkpol is vastly dominating the distribution of hashtags. Around one third of all tweets by Danish politicians include this hashtag. Several hashtags created by various news media seem to by popular. For example, the top 10 includes #fv15, #ftlive and #tv2valg as popular hashtags.<br><br>
                But how do the parties actually differ? We can use tfidf to seperate the hashtags of each party and gain knowledge of the unique keywords for each individual party.</p>

                <h2>What do parties say with their #hashtags?</h2>
                <div class="img-car">
                    <div class="single-item">
                        <img src="img/wordcloud/alt.png" alt="">
                        <p>Alternativet's hashtags (top tfidf as sizes)</p>
                    </div>
                    <div class="single-item">
                        <img src="img/wordcloud/df.png" alt="">
                        <p>Dansk Folkeparti's hashtags (top tfidf as sizes)</p>
                    </div>
                    <div class="single-item">
                        <img src="img/wordcloud/el.png" alt="">
                        <p>Enhedslisten's hashtags (top tfidf as sizes)</p>
                    </div>
                    <div class="single-item">
                        <img src="img/wordcloud/kon.png" alt="">
                        <p>De Konservative's hashtags (top tfidf as sizes)</p>
                    </div>
                    <div class="single-item">
                        <img src="img/wordcloud/la.png" alt="">
                        <p>Liberal Alliance's hashtags (top tfidf as sizes)</p>
                    </div>
                    <div class="single-item">
                        <img src="img/wordcloud/r.png" alt="">
                        <p>Radikale Venstre's hashtags (top tfidf as sizes)</p>
                    </div>
                    <div class="single-item">
                        <img src="img/wordcloud/s.png" alt="">
                        <p>Socialdemokratiet's hashtags (top tfidf as sizes)</p>
                    </div>
                    <div class="single-item">
                        <img src="img/wordcloud/sf.png" alt="">
                        <p>Socialistisk Folkeparti's hashtags (top tfidf as sizes)</p>
                    </div>
                    <div class="single-item">
                        <img src="img/wordcloud/v.png" alt="">
                        <p>Venstre's hashtags (top tfidf as sizes)</p>
                    </div>
                </div>
                <p>The wordsclouds does capture phrases commonly associated with the parties. Examples are Alternativet,
                which tends to use hashtags such as #venligrevolution, #elbil, and #nypolitiskkultur, and Dansk Folkeparti,
                which include hashtags such as #meredkmindreeu, #grænsekontrol, and #sønderjylland among its defining hashtags.</p><br>
            </div>

## Motivation

Relationship between disneys movies.


## Download link
[Data for project](https://github.com/signemik/SocialGraphsAnimateMovies/blob/main/Download/Movie_Data.xlsx?raw=true)








<!--
## Welcome to GitHub Pages
<!--
You can use the [editor on GitHub](https://github.com/signemik/SocailGraphsAnimateMovies/edit/main/README.md) to maintain and preview the content for your website in Markdown files.
<!--
Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.
<!--
### Markdown
<!--
Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for
<!--
```markdown
Syntax highlighted code block
<!--
# Header 1
## Header 2
### Header 3
<!--
- Bulleted
- List
<!--
1. Numbered
2. List
<!--
**Bold** and _Italic_ and `Code` text
<!--
## Images
<img src="Images/DTU.png" height="100"> 
<!--This is a comment-->
<!--![](Images/DTU.png)-->
<!--
[Link](url) and ![Image](src)
```
<!--
For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).
<!--
### Jekyll Themes
<!--
Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/signemik/SocailGraphsAnimateMovies/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file. -->
<!--
### Support or Contact
<!--
Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
