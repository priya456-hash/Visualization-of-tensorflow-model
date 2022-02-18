# Visualization-of-tensorflow-model
Sequential model is created using Tensorflow and graphviz is used for visualization purpose. 

For model creation, adam optimizer and cross entropy as loss function are used. 
#model creation
model = Sequential()
model.add(layers.Dense(4, input_shape = (8,), activation = 'relu' ))
model.add(layers.Dense(8, activation='relu'))
model.add(layers.Dense(8, activation='relu'))
model.add(layers.Dense(8, activation='relu'))
model.add(layers.Dense(8, activation='relu'))
model.add(layers.Dense(8, activation='relu'))
model.compile(optimizer = 'adam', loss = 'crossentropy', metrics= ['accuracy'])

first layer neurons are visualized 

![image](https://user-images.githubusercontent.com/74081639/154751119-f616574c-252f-4424-8608-c8737eb1b67d.png)

Connection between input and hidden layer are visulaized with the creation edge list 
![image](https://user-images.githubusercontent.com/74081639/154750812-4f901ead-050c-4b21-a722-c5bb6028a5c9.png)

