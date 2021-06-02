# Development of Efficient Electricity Distribution Model

### Course: Algorithm Analysis and Design

## Team AM
- Aryan Kharbanda (2019101018)
- Mayank Jain (2019101023)
- Umang Srivastava (2019101090)
- Arth Raj (2019101094)
- Kshitij Mishra (2019111014)

## Overview

Electricity companies face a lot of issues regarding the efficient power supply to all their
customers as well as the customers have issues regarding their needs of power especially
during peak hours.
Our aim is to develop and implement algorithms to improve this situation and implement
better, renewable resources for generation of electricity at household level (two way
transmission).
For companies to increase their profit margin, we implemented dynamic pricing.

### SUGGESTIONS BY PROFESSOR AND MENTOR

● Develop a dynamic pricing model
● Develop a two-way electricity distribution model where the consumer can also supply in
specific scenarios

### CHALLENGES

1. Clustering of Houses
2. Load Shedding
3. Static and Dynamic Pricing
4. Two-way electricity Distribution


## Clustering of Houses

Most of the residential colonies and areas in India are scattered and don't follow a specific
distribution, while western countries have a well planned city layout and structure. Hence it
becomes a problem in India to cluster houses in an area which follows a specific pattern of
electricity consumption.

### GOAL

To make clusters of houses which are near to each other in a city by making localities.

### SOLUTION

KMeans algorithm has been used to address the problem. We use geographical coordinates
of a given set of houses as inputs. KMeans algorithm is an iterative algorithm that tries to
partition the dataset into k pre-defined distinct non-overlapping subgroups (clusters) where
each data point belongs to only one group. We categorize these houses into groups.

### DESIGN

The algorithm works as follows:
● First we initialize k points, called means, randomly.
● We categorize each item to its closest mean and we update the mean’s coordinates,
which are the averages of the items categorized in that mean so far.
● We repeat the process for a given number of iterations and at the end, we have our
clusters

## Load Shedding

### PROBLEM

The second major problem related to electricity in India is unavailability of required amounts
of electricity. While western grid and southern grid are surplus with electricity, northern and
eastern grids are production deficits. This is solely due to large demand for electricity in
households during peak hours of the day. This problem is dealt with by illogically cutting
powers of localities. Can we find mathematical ways to find localities to manage this?

### GOALS

● Finding an algorithm which helps in solving the above mentioned problem.
● Making the algorithm work for the clusters of houses so that load shedding can be
done.

### SOLUTION

Our first approach is the ​ **Greedy algorithm** ​ to minimise the number of houses to be cut-off.
Meters in houses calculate the current power consumption and with this data, greedy can be
applied. A better approach would be to maximise profit by using ​ **Knapsack algorithm** ​. Values
of weight and benefit will be analogous to current consumption and profit, which is calculated
by multiplying the consumption with respective prices according to the meter installed.
Arbitrary data : ₹ 4 for 2 kW meter, ₹ 4. 5 for 5 kW meter and ₹ 6 for 10 kW meter. Considering the
larger scale on which these algorithms will be applied, it is better for the company to cut off
the entire cluster (all houses connected to a transformer). This is carried out by Knapsack
using weight and benefit as the cumulative consumption and profit for a cluster. This process
is repeated after fixed intervals so we get new sets of localities which must be provided with


## Pricing Model

### PROBLEM

The traditional pricing model followed for consumers is based upon the slots which depends
on consumption. For instance, 10 - 100 units cost ​₹​x, then 100 - 150 units cost ​₹y ​and so on. This
slab based pricing method does not account for wastage of electricity as well as very uneven
pricing based on consumption demands. It is logical to decide price based on consumption
demands as different topography has different consumption patterns.

### GOALS

● Develop 2 pricing models: Static and Dynamic.
● Base the pricing on the consumption pattern of a cluster rather than a fixed slab.

### SOLUTION

We develop two pricing models: Static Pricing and Dynamic Pricing. Static Pricing includes
different slabs that have a fixed price per unit and is used for houses that opt for it. Dynamic
Pricing depends on various factors like the cost of production, fuel costs, infrastructure costs,
etc. The city is divided into clusters of static and dynamic pricing, each applied to clusters
based on the consumer demands.

## Two - Way distribution of Electricity

### PROBLEM

Under normal distribution method, there is one supplier and many consumers. That is, the
relationship for supply to demand is one to many. This has several drawbacks as there is
much load on one head as well as there is no promotion of renewable sources of energy on
grass root level. In this modern era, the focus is on futuristic sources of energy, minimising
wastage and pollution that occurs during production of electricity.

### GOALS

● Develop a two-way electricity distribution system where the consumer itself can produce
electricity.
● Implement futuristic methods of production of electricity.

### SOLUTION

We design a two-way electricity distribution model where the consumer ( by renewable
methods like solar energy) can distribute in its cluster when the demand increases. This not
only reduces the demand load on the supplier but is also beneficial for the environment. Also,
this reduces the bill for the consumer as it can use the electricity developed in-house.

