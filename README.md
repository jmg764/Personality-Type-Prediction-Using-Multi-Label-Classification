# Predicting-Personality-from-Text-An-Analysis-of-Multi-Label-Classification-Methods
## Background
Carl Jung, founder of the field of analytical psychology, formulated a personality theory aiming to categorize people based on how they process information. He identified two types of cognitive functions: two perception functions known as sensation and intuition, and two judgement functions known as thinking and feeling. The functions within each pair are considered to be opposites of each other. 

<p align="center">
  <img src="images/cognitive_functions_diagram.png"  alt="drawing" width="325"/>
</p>

Additionally, these four functions operate in conjunction with either an introverted or extroverted attitude. This results in eight functional variations, or personality types: extroverted sensing (Se), introverted sensing(Si), extroverted intuition (Ne), introverted intuition (Ni), extroverted feeling (Fe), introverted feeling (Fi), extroverted thinking (Te), and introverted thinking (Ti). 

All four cognitive functions are used at different times depending on the circumstances. However, one of the four functions tend to be used more frequently than the other three in a more conscious and confident way. This dominant function is supported by two auxiliary functions. The dominant and first auxiliary are referred to as the two primary cognitive functions, and are of different cognitive function type: for example, if the dominant function is a judging type, then the first auxillary will be a perceiving type and vice versa. The fourth and least conscious function, often referred to as the inferior function, is always the opposite of the dominant function in terms of cognitive function and attitude. For example, an extroverted thinking dominant function would be balanced by an introverted feeling inferior function. Jung theorized that the dominant function characterizes conscious behavior, while the inferior function is repressed and characterizes unconscious behavior.

Jung's personality theory formed the basis of the Myers-Briggs Type Indicator (MBTI) which is a widely used method of self-categorization of personality type through an introspective questionnaire. The relationships between MBTI type and Jungian cognitive functions are shown below. Primary cognitive functions are highlighted in green.

<p align="center">
  <img src="images/mbti_cognitive_functions_relationship.png"  alt="drawing" width="175"/>
</p>

## Objective
The objective is to develop a machine learning model which can can accurately predict a person's two primary cognitive functions based off of what they have written. In doing so, the following multi-label classification techniques are implemented and compared: 

<ol start="1">
  <li><b>Problem transformation, algorithm adaptation, and ensemble approaches</b></li>
 
<ol type="a">
  <li>Problem transformation approaches</li>
    <ul type="disc">
      <li>Binary relevance</li>
      <li>Classifier chain</li>
      <li>Label powerset</li>
    </ul>
  <li>Algorithm adaptation approaches</li>
    <ul type="disc">
        <li>Multi-label k-nearest neighbors (MLkNN)</li> 
        <li>Multi-label hierarchical ARAM neural network (MLARAM)</li>  
    </ul>
    <li>Ensembles of classifiers</li>
    <ul type="disc">
        <li>Random label space partitioning with label powerset (RAkELd)</li>  
    </ul>
</ol>
  <li><b>Neural networks using Keras</b></li>
    <ul type="disc">
      <li>Long short-term memory networks (LSTM)</li>
      <li>1D convolutional neural networks (CNN)</li>
    </ul>
  <li><b>Bidirectional Encoder Representations from Transformers (BERT)</b></li>
  </ol>

The [dataset](https://data.world/just4jcgeorge/myers-briggs-personality-type-test-dataset) used contains a large selection of people's MBTI personality types and text they have written on a forum called Personality Cafe: a community dedicated to discussion about personality types.
