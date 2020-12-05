# Shop the Look: Fashion Compatibility Prediction for Complementary Product Recommendation
Luisa PolanÌa Cabrera, Principal AI Scientist, Target

### Notes
* Trying to recommend a look
* Example - if you are looking to buy jacket, get recommendations for pants or tops to go with it
* Using 2 dataset - 
  * Polyvore dataset: popular fashion oriented website that provide interfaces for users to create fashion outfit
  * Target images - internal data; information about items in the image like TIN
* Using siamese network - need positive and negative pairs
  * positive pairs - all possible combinations of compatible pairs formed by training / validation outfits
  * negative pairs - randomly select items from different outfit
* Changing siamese model - add color features; make fully connected network to generate more complex compatibility functions; formulating as MAP
(maximum-a-posteriori) problem.
* Once you train the model, you take all the items in catalogue and generate embeddings for each image
* Then customer select a seed, that is, one of the item
  * for example, a top
  * then look for the top in the embeddings
  * if it is there, use siamese model to generate the matching outwear
  * return outerwear with top score
  * repeat for pants
* Metrics - New model results are better than traditional siamese model
* Outfit recommendations by occasion and style: How to style one outfit for evening day / work / vacation / day out
* Apply model to other categories - outfit recommendation for kids / men / furniture set
