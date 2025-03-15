# emotion_generation

Difference between latent spaces : 

Z : initial
W : intermediate
W^+ : extension of W : different copy of w \in W for each layer of the generator (which will then be fed into Affine transformations to produce styles)
S : style space

Expériences pour les posters : 

    - Global demonstration : 5 neutral faces -> several emotions
    - Emotion classification : non-explicit prompts, with vs withous classifier in the loss
    - Custom evaluation metric on the image inversion (original vs ours)
    - Custom evaluation metric with different truncation values

Personal contributions : 

    - combination of e4e and gradient descent for image inversion
    - emotion classifier in the loss of the gradient descent for edition
    - evaluation metric : combination of ID_loss, FID and emotion classification