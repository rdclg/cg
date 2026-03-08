import matplotlib.pyplot as plt   # this is used for drawing

\# Step 2: Make a blank page

plt.figure(figsize=(4,4) )                     # this opens an empty drawing page

\# Step 3: Draw a line

plt.plot(\[1, 4], \[1, 4])          # line from point (1,1) to point (4,4)

\# Step 4: Draw a circle

circle = plt.Circle((2, 2), 1, fill=False)   # (2,2)= circle center, 1=radius

plt.gca().add\_patch(circle)       # place the circle on the pageplt,gca() means

&nbsp;                                                    #Get the current drawing area.”

\# Step 5: Draw a rectangle

rect = plt.Rectangle((4, 1), 2, 1, fill=False)   # (4,1)=corner, 2=width, 1=height

plt.gca().add\_patch(rect)         # place the rectangle on the page

\# Step 6: Draw a triangle

triangle = plt.Polygon(\[\[1,1], \[2,3], \[3,1]], fill=False)   # 3 corner points

plt.gca().add\_patch(triangle)     # place the triangle on the page

\# Step 7: Show everything

plt.axis('equal')                 # keep shapes proper

plt.show()                        # show the drawing window







