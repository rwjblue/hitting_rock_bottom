#Basic Concept
The water flows in from the top left of the cave and flows down the wall
the over to the next barrier. At that point it will begin to rise to the
level of the barrier.

#Goal
The goal is to accept an input cave layout in ASCII ('#' is a wall), and
the number of water 'units'. Then output the total depth of water for each
column in the cave.

#Rules of Governance

1. The stream of water must remain continuous.
2. The water flows all the way down before it starts spreading from left to right.


#Example Input & Flow Pattern

Initial state:

    ###########################
    ~                         #
    #                         #
    #                         #
    #         ####            #
    #         ####            #
    #         ####            #
    ###########################

Water begins flowing down the wall:

    ###########################
    ~~                        #
    #~                        #
    #~                        #
    #~       ####             #
    #~       ####             #
    #~       ####             #
    ###########################

Once it hits bottom it flows right until hitting a wall:

    ###########################
    ~~                        #
    #~                        #
    #~                        #
    #~       ####             #
    #~       ####             #
    #~~~~~~~~####             #
    ###########################

Then it starts to rise one level and spreading to the right again:

    ###########################
    ~~                        #
    #~                        #
    #~                        #
    #~       ####             #
    #~~~~~~~~####             #
    #~~~~~~~~####             #
    ###########################
