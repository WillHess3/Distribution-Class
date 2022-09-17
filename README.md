# Distribution-Class
This is the class that helped me make the customizable distributions in "the most random battle" (part 1) 

to use the class, first make 2 lists of equal counts (things will probobly break otherwise). Populate your first list with items you want in the distribution, and then populate the second list with floats of the probability of getting the corresponding item. 

For example:
if I want a sword to drop 20% of the time, then
_items[0] = sword;
_dropChance[0] = .2f;
MAKE SURE ALL YOUR PROBABILITIES (elements in the float list) SUM TO 1

Next make a new distribution and pass in your two lists as arguments.
Distribution<Item> _distribution = new Distribution<Item>(_items, _dropChance);

Now all you have to do to get a random item from the distribution is do
_distribution.RandomFromDistribution();
