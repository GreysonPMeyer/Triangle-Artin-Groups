# Computing Fiber Products In Pursuit of S

  Fiber_Product.py is a python program that computes the fiber products necessary in the construction of the set S for the triangle Artin group A_{2,3,8} from the paper https://arxiv.org/abs/2412.07063. The relevant graphs are represented by the variables W, Y1, bY1, Y2, Y3, bY3 and Y4. The build_F3 function allows the user to view each of graphs as a graphic made with the turtle package.

  To explore the connected components of the fiber product of a pair from this set of graphs, pass the pair of graphs into the check_fiber function. The check_fiber function performs
the fiber product of the input graphs, then uses the split function to create a dictionary of the connected components of the fiber product. You will then be prompted to choose a key
from this dictionary, which will then be created by the turtle for your viewing. Furthermore, check_fiber returns a piece of text that informs you of which graph this connected component is a subgraph of, or if it is contractible under q. It will also reveal how many connected components of this fiber product are subgraphs of the red square in W, and how many are subgraphs of the green-yellow triangle in W.

  If you would like to check an entire row of the table on page 26 in https://arxiv.org/abs/2412.07063, use the check_row function. This function perofrms the fiber product, splits the fiber product into its connected components, and then counts the number of connected components that are subgraphs of the relevant set of graphs, as well as how many connected components are q-contractible.

  Lastly, Y4 x Y4 is a calculation that results in a fiber product that takes quite a bit of time to break into its connected components. A dictionary of the connected components of
Y4 x Y4 is included in the file so that this calculation need not necessarily be run. Since this dictionary is included in the file, to check the Y4 x Y4 row in the table, it is
recommended that you apply the check_row_Y4xY4 function to the dictionary Y4_x_Y4.
