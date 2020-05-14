# brain-cell-clusterer

## Aim of project

Project using unsupervised learning to cluster brain cells and find genetic markers for each cluster

## Goal
Brain cells (neurons) come in millions of shapes and sizes. Even neurons that are right next to each other in the brain can carry out completely different functions! It is useful for scientists to be able to identify, and find markers for, groups of neurons in the brain that might carry out the same function. Scientists can then use this information to discover more about how these neurons work in both healthy people and models of disease.

## Process

1. The script takes as its input a **.csv** file with rows=genes and columns=neurons. Each cell in the table contains the RNA transcript copy numbers (obtained via single nuclei RNA sequencing) for a particular gene for a particular neuron

2. The script carries out the following steps:

    - loads data and finds genes that are highly variable (i.e. that are expressed highly in some neurons but lowly in others)
    - carries out a principal components analysis to reduce the dimensionality of the data
    - uses principal components from previous step to cluster the neurons using K-means clustering
    - finds genetic markers for clusters

## Requirements

- use Python 3
- required libraries listed in requirements.txt
