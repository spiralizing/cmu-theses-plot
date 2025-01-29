# What am I looking at? 
## Introducing the KiltHub Thesis Explorer 🔭
Ever wondered how your research connects to work across different departments? Curious about unexplored areas in your field? We're excited to introduce a new interactive visualization tool that maps the entire landscape of graduate research at CMU!

## What You'll See 👀
Imagine a star map, but instead of stars, you're looking at every graduate thesis in KiltHub. Each point represents a thesis, and the space between them shows how related their topics are – the closer together, the more similar their research themes. This creates a fascinating "galaxy" of CMU graduate research where you can:
- Discover unexpected connections between different fields  
- Find potential collaborators across departments  
- Identify unique research opportunities  
- Explore the evolution of research themes across colleges

## How to Explore 🔍
### Interactive Features  
- ***Zoom:*** Like Google Maps, but for research! Zoom in to explore specific research clusters or out to see the big picture  
- ***Hover:*** Mouse over any point to see thesis details, including:  
  - Title  
  - College  
  - Research topics  
- ***Filter:*** Click on college names to show or hide different departments 

### Research Insights ⚛️  
- Find clusters of related work across different colleges  
- Spot gaps between fields that might inspire new research directions  
- Identify potential interdisciplinary collaboration opportunities  
- See how your research interests connect to other fields

## Behind the Scenes 🛠️
This visualization was created using state-of-the-art natural language processing techniques that transform thesis abstracts into a semantic map. Think of it as a GPS system for research topics – it captures the *semantic* meaning of the research, not just keywords, allowing it to show conceptual relationships between different works.

## Ready to Explore? ⭐
Visit --- or scan the QR code to start exploring the CMU's graduate theses landscape! 
*We recommend open the webpage on your computer for a better experience*

## Technical Details  
**Feature Extraction**: Count vectorizer followed by Class-based TF-IDF transformation  
**Embedding Model**: \`paraphrase-MiniLM-L6-v2\` from [sentence-transformers](https://huggingface.co/sentence-transformers) to generate 384-dimensional embeddings of thesis descriptions  
**Clustering Method**: [HDBSCAN](https://hdbscan.readthedocs.io/en/latest/index.html) to assign points to clusters in the embedding space  
**Dimensionality Reduction**: We used [UMAP](https://umap-learn.readthedocs.io/en/latest/) to reduce from 384 to 2 dimensions for visualization purposes

### Acknowledgements
We used [BERTopic](https://maartengr.github.io/BERTopic/) to develop the workflow for this project.

---------------
*This project is a collaboration between the University Libraries and the Tartan Research Data Alliance. Built with love for the Love Data Week 2025 and the CMU community.*

TRDA members: Chekah Arora and Alfredo González-Espinoza`;
