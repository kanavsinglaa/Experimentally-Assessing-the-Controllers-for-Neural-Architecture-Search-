# Experimentally-Assessing-the-Controllers-for-Neural-Architecture-Search-
Neural networks are powerful and flexible models that work well for many complicated tasks such as computer vision, text & speech processing, combinatorial optimization problems, etc. “AI that creates AI”, was a common headline of what people initially described as Automated Machine Learning (i.e. Auto ML). This novel concept gained attraction in 2016 when Google Brain released their first “Neural Architecture Search with Reinforcement Learning (NAS)”. Traditionally, choosing a neural network architecture manually is a tiring, inefficient & computationally expensive task. Even the standard NAS is very computationally expensive as it required over 450 GPU’s for 3-4 days to train on CIFAR-10. We are analyzing & reproducing the method of standard Neural Architecture Search (NAS) through an existing improved method known as “Efficient Neural Architecture Search via Parameter Sharing (ENAS)”. We are assessing the quality of the ENAS architectures’ RNN controller using different experimental techniques such as search space poisoning and random search to see how the controller performs when decoupled with strong search spaces. 
#### Please drop a star if you find this helpful or atleast mildly exciting ;)

### Macro Search on the architecture looks like:
<p align="center">
  <img src="GIFS/MacroSearch.gif" alt="animated" />
</p>


#### The RNN (LSTM) controller trained on REINFORCE outputs a CNN below to classify CIFAR-10 data in different categories. Note that after the initial controller settings, no human involvement is required to produce these child networks. These CNN networks are purely produced by the RNN Contoller, which essentially learns which search space options are better than others and how different combinations would result in better accuracies for the child network.

### This is essentially training a Neural Network to produce a Neural Network. Creating AI which further creates AI!
To understand how this works in detail, read our paper attached above.
