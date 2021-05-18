# task_planner

In this application, user will feed the tasks to do and their dependencies.\

Based on these, application will generate the order in which given tasks can be executed. \

# Directory Structure
1. data holds all the data\
2. engine holds the algorithms\
3. result holds the output\


# Thoughts. 
1. Ask user to list down all the tasks she/he needs to work on. \
    Ex:\
        >> Have bath\
        >> Wear clothes\
        >> Brush the teeth\
        >> Go to office\
        >> Drink Coffee\

2. After all the tasks are entered, display the tasks on the screen with all numbers beside them. \
    Ex:\
        1. Have bath\
        2. Wear clothes\
        3. Brush the teeth\
        4. Go to office\
        5. Drink Coffee\

3. Now user enters a 2D list showing dependencies while referring to the tasks mentioned above\
    Ex:\
        before "a" you need to do "b" [a,b]\
        [[1,3],[2,1],[4,1],[4,2]]\

4. Based on this 2D list, topo output is displayed.\
    Ex:\
        3. Brush the teeth\
        1. Have bath\
        2. Wear clothes\
        4. Go to office\
        5. Drink Coffee\

we could use https://networkx.org/ to draw/display the final graph (also re-assign new numbers to the tasks)\
