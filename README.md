# Smart-Reply-with-TensorFlow-Lite

This model generates reply suggestions based on input conversational chat messages.

Smart Replies are one touch responses that make replying to a text/email faster and more convenient for a user. This model, built using the TensorFlow Lite library, generates multiple contextually relevant suggestions for a given input message allowing the user to easily reply to an incoming message. TensorFlow Lite is a mobile library used for deploying models on microcontrollers, mobiles etc.
The given input is initially preprocessed which includes steps such as sentence splitting, normalization (converting to lowercase, removing punctuations, etc.), and extracting the features from the input to finally get input tensors. These input tensors are fed to a prediction model which generates a list of possible responses. Responses are sorted in descending order of confidence score. In case no responses are triggered, the model outputs responses from a fixed list of pre-set fallback replies such as Yes, No, Okay etc.
The triggering rate (the percentage of times the model suggests a response for an incoming message) of this model is close to 50%.
