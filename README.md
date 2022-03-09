# Art&Emotions (Emotions Evoked from Colors of Paintings)

## Introduction & The Question
Artists often use color as a medium to convey different messages, feelings, and symbolisms. The artists’ use of different colors and shades can greatly influence how the viewer perceives a painting and what they take away from it. My Arts & Emotions project aims to provide a bridge between paintings and the emotions they evoke within us when we look at them. By explaining how different colors impact the human psyche I aim to help people understand why artists make the color choices they do and why as viewers we feel a certain way when looking at a painting




## Dataset
- WikiArt-info.tsv = original dataset before adding columns
- output.csv = csv file for the images url 
- full_emotion_color.csv = added columns to WikiArt-info.tsv 
- emotions_images.csv = has emotions and colors dataset


## Data Dictionary 

<ul>
<li><i>ID</i>:    <i>Painting ID</i></li>
<li><i>Category</i>: <i>Painting style (Impressionism, realism, cubism .. etc)</i></li>
<li><i>Artist</i>: <i>The painting's artist's name</i></li>
<li><i>Title</i>: <i>The title of the Painting </i></li>
<li><i>Year</i>: <i>The year of the painting</i></li>
<li><i>Image URL</i>: <i>URL of the website that contains the image /i></li>
<li><i>Painting Info URLe </i>: <i>Info of the painting link</i></li>
<li><i>Artist Info URL</i>: <i>Info on the artist link </i></li>


</ul>
<br>

Added Columns 

- dcolor = dominant color in RGB format
- rgb = a palette of the colors used in the painting in RGB format
- palette = each of the color palettes names
- dcname =  the name of the dominant color 
                     



## Resources
https://www.wikiart.org/  <br>
https://core.ac.uk/download/pdf/153368581.pdf  <br>
https://medium.com/artificialis/extracting-and-analyzing-colors-from-images-with-python-3a762ee1c3d7
https://raw.githubusercontent.com/josh-ashkinaze/Emotion-Colors/master/emotions_images.csv


## Project approach & solution

My project works by putting images of paintings in color clusters and classifying them with emotions. Look below for more details.
I used kmean algorithm to cluster my images & knn classifier & Random Forest

emotions_images.csv: for this dataset since it has emotions and colors, I added a column for the colors name & RGB to compare my dataset with this one and get the emotions but when I ran the classifier on this dataset it wasnt accurate since it was scraping images of shocking expressions and different expressions but not scraping images that focus on colors, which is why I found that clustering is the approach for this. since I don't have a dataset to classify (supervised learning), the approach to this is using clustering the colors (unsupervised learning)

## conclusion


<ul>
<li> This project allows me to combine topics that are meaningful to me: Data Science, Art, and Psychology </li>
  <li> Colors in paintings and all around in our everyday lives influence our emotions and perception </li>
  <li> Understanding how what positive or negative effect different colors have allows us to use them as a tool to express ourselves </li>
</ul>
<br>






## Future Development


<ul>
<li> Extract Emotions from Title & Painting Description using NLP </li>
  <li> Portrait & Landscape Paitings Classifier </li>
  <li> Extract emotion from face expressions in portrait paintings </li>
  <li> For the abstract/landscape paintings, I will analyze the lines & shapes</li>
</ul>
<br>

Lines: <br>
A dark, thick, angled line show anger or being mad <br>
A thin, flowing, rounded line show happiness


Shapes: <br>
Squares, triangles and rectangles can show anger, fear, confusion <br>
Ovals can show sadness <br>
Circles can show happiness and joy


## Limitations
My code was taking a long time to run when doing image processing 






