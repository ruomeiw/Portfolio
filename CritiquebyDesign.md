# Assignment 3 & 4: Critique by Design
## Original Visualization
<img width="800" alt="billboard" src="https://user-images.githubusercontent.com/107513376/201799595-bdeb176b-ecb5-40a2-8135-065869b34660.png">

Link to the original visualization is [here](https://github.com/gkaramanis/tidytuesday/tree/master/2021/2021-week37)
<br>
Original Dataset can be downloaded from [Data.World](https://data.world/kcmillersean/billboard-hot-100-1958-2017#)

## My Process
My favorite hobby is discovering excellent music, and I've always been passionate in learning about all of the different musical genres. So I started looking for graphics related to music when I needed to discover data visualizations to analyze and develop. I discovered the original data visualization seen above. Although the visualization is **already fantastic**, I think it might be even better.

* The color scheme and the genre labels in this data visualization caught my attention the most at first glance. The rainbow-like color scheme is attractive and does a great job at drawing audiences. The categories of the genres, however, progressively start to have similar colors and merge towards the top and bottom of the picture, making it fairly difficult for the viewer to distinguish between them. I would work to distinguish between different genres so that it would be simpler for the audience to recognize each one at a glance.

* Second, the genre labels distinguished each genre category, but the font size was too small in certain spots, making it difficult for human eyes to read. Additionally, the representation is quite noisy and confusing due to the quantity of labels. To simplify the representation, I would do away with the labels and use titles to identify each genre. In addition, I'll display the proportion of each genre in each year to illustrate both the proportion and any changes or trends.

* Third, to reach the primary audience more effectively, we need to provide more specific figures or percentages. 

Using the **Data Visualization Effectiveness Profile**, I am able to define and discuss what is missing in this visualization. This visualization has many positive qualities that we can learn from (high data truthfulness, technological data processing techniques, etc.), but it also has several drawbacks that could be fixed. I can also pinpoint who the visualization is intended for: anyone curious to know more about how the best known musical genres have changed over the course of the Billboard Hot 100 from 1958 to 2021.The primary audience are music ethusiastic who focuses on the details of the music industry, and they aim for more detailed and specific information.

I started analyzing the raw data I had downloaded from Data.World with all these considerations in mind. The raw data is complicated since the music genres of each song are layered together in a single Excel cell. I wrote a *Python program* to process the data in order to separate and extract each and every genre. The data was then loaded into Tableau.

## My Sketches and User Feedback
This is the first sketch I created using Tableau.
<br>
<div class='tableauPlaceholder' id='viz1668475101838' style='position: relative'>
  <noscript>
    <a href='#'><img alt='Music Genres of the Billboard Hot 100 ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Mu&#47;MusicGenresoftheBillboardHot100&#47;Sheet1&#47;1_rss.png' style='border: none' />
    </a>
  </noscript>
  <object class='tableauViz'  style='display:none;'>
    <param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' />
    <param name='embed_code_version' value='3' />
    <param name='site_root' value='' />
    <param name='name' value='MusicGenresoftheBillboardHot100&#47;Sheet1' />
    <param name='tabs' value='no' />
    <param name='toolbar' value='yes' />
    <param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Mu&#47;MusicGenresoftheBillboardHot100&#47;Sheet1&#47;1.png' /> 
    <param name='animate_transition' value='yes' />
    <param name='display_static_image' value='yes' />
    <param name='display_spinner' value='yes' />
    <param name='display_overlay' value='yes' />
    <param name='language' value='en-US' />
  </object>
</div>                
<script type='text/javascript'>                    
  var divElement = document.getElementById('viz1668475101838');                    
  var vizElement = divElement.getElementsByTagName('object')[0];                    
  vizElement.style.width='100%';
  vizElement.style.height=(divElement.offsetWidth*0.75)+'px';                    
  var scriptElement = document.createElement('script');                    
  scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    
  vizElement.parentNode.insertBefore(scriptElement, vizElement);                
</script>

<br>
I displayed my initial sketch to two friends, one of whom is currently taking this course and the other who took it last semester. According to feedback, this graphic is simpler than the original, but because there are so many genres covered, many of them are no longer showing in this Tree Map. They also said I should focus on the top 100 genres because people might not be interested in knowing about so many others.

<br>
After that, I drew my second sketch.
<br>
<div class='tableauPlaceholder' id='viz1668475236756' style='position: relative'>
  <noscript>
    <a href='#'>
  <img alt='Top 100 Music Genres of the Billboard Hot 100 ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;To&#47;Top100MusicGenresoftheBillboardHot100&#47;Sheet2&#47;1_rss.png' style='border: none' />
  </a>
  </noscript>
  <object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> 
    <param name='embed_code_version' value='3' />
    <param name='site_root' value='' />
    <param name='name' value='Top100MusicGenresoftheBillboardHot100&#47;Sheet2' />
    <param name='tabs' value='no' />
    <param name='toolbar' value='yes' />
    <param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;To&#47;Top100MusicGenresoftheBillboardHot100&#47;Sheet2&#47;1.png' /> 
    <param name='animate_transition' value='yes' />
    <param name='display_static_image' value='yes' />
    <param name='display_spinner' value='yes' />
    <param name='display_overlay' value='yes' />
    <param name='language' value='en-US' />
  </object>
</div>                
<script type='text/javascript'>                    
  var divElement = document.getElementById('viz1668475236756');                    
  var vizElement = divElement.getElementsByTagName('object')[0];                    
  vizElement.style.width='100%';
  vizElement.style.height=(divElement.offsetWidth*0.75)+'px';                    
  var scriptElement = document.createElement('script');                    
  scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    
  vizElement.parentNode.insertBefore(scriptElement, vizElement);                
</script>
<br>
This time, all the labels are visible and only the top 100 genres are listed. When I reintroduced this to my audience, they suggested that I consider including the year like the original graphic.

<br>
Then I used Flourish Studio to produce a new graphic. The disparities between the data points, however, are so great that only a few categories are showing results in the 50% to 60% range, while the remainder are still floating around 0%. I realize that a single line chart might not be the best option.
<br><br>
<img width="900" alt="Wireframe3" src="https://user-images.githubusercontent.com/107513376/201801969-1819257a-dfe3-4676-ac2c-8132c115f23f.PNG">

## Final Redesigned Data Visualization
The updated data visualization I came up with is shown below. It is **unambiguous, straightforward, interactive, and simple to read**. 
Only the top 100 genres are presented, and each genre has its own stacked area chart with year labels so that viewers can easily understand how each genre has changed over time and which ones are among the most popular. For instance, the most popular genres are the first two rows, and they consistently appear in the charts; other genres, like hard rock, occasionally go off the chart.
<div class="flourish-embed flourish-chart" data-src="visualisation/11817597"><script src="https://public.flourish.studio/resources/embed.js"></script></div>

## My Takeaway
I had no idea that we could make this many diverse visualizations utilizing the same data set before this critiquing assignment. Because I love this topic and have learned so much more about different music genres, I also had a lot of fun making the sketches. I'm also impressed by how drastically the storytelling may alter with only a small tweak to the graphic.


## [< Go back to the main page](/README.md)
