### first half of the session
- what is programming 
- how is traditional programming diff from ai programming?
    - ai - data driven 
    - harness for deployment algorithm 
- diff types of ML
- neural networks
- vocabulary

# Hands-On

https://colab.research.google.com/drive/1zuYDY4sWIu9TEO-Xxxrl5iAGyfvV0pKH#scrollTo=uGFBU32r5D1d

- jupyter notebook 
    - html program
    - python program
    - has a python kernel running in the bg

- google collab

- simple linear regression problem
    - y=mx+c
    - y=wc+b
        w -> weights
        b -> bias


        import numpy as np
        import matplotlib.pyplot as plt
        from sklearn.model_selection import train_test_split
        from sklearn.linear_model import LinearRegression
        from sklearn.metrics import mean_squared_error

        # Create the dataset
        data = [(1, 2), (2, 4), (4, 8), (5, 10), (10, 20)]

        # Separate features (a) and labels (b)
        X = np.array([row[0] for row in data]).reshape(-1, 1)  # Feature vector
        y = np.array([row[1] for row in data])  # Label+

        # Split the data into training and testing sets
        X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42)

        # Create a linear regression model
        model = LinearRegression()

        # Train the model
        model.fit(X_train, y_train)

        # Make predictions on the test set
        y_pred = model.predict(X_test)

        # Evaluate the model
        mse = mean_squared_error(y_test, y_pred)
        print("Mean Squared Error:", mse)

        # Print the model's coefficients
        print("Intercept:", model.intercept_)
        print("Coefficient:", model.coef_)


    - after running 
        Mean Squared Error: 0.0
        Intercept: 0.0
        Coefficient: [2.]



    - in regression we see mean square error 
    - if mean square is a non zero value- it depends on how good or bad the model is
    - we dont use regression to predict usually 


    - Using Tensorflow
        - stochastic gradient
        - numpy - for arrays
        - helps data run on gpus better - tensorflow
        - adding noise by + np.random.rand(100,1)

    ### check the google colab out

### https://colab.research.google.com/drive/1xdpTNTQ7N63wbAxTvRQi9rS7zg5SZkVP
- polynomial regression

- first install !pip install ucimlrepo
- uci dataset, import in python
- use genai to figure out how to implement various algorithms



#MNIST dataset
- we have handwritten data 
- we are trying to push it through a neural network
- input : 28*28 grey scaled image
- output : 784 - flatten it
- 128 neurons
- connecting to 10 more neurons
- dense connection
- training accuracy 98
- validation accuracy 97


- convolution neural network 
    - spatial info
    - 