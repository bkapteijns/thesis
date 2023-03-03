The latest file is 'nlp_shap.ipynb'. The current problem is that TransSHAP does not work yet. Running code block 57 (with line `shap_values = explainer.shap_values(X=to_use, nsamples=64, l1_reg="aic")`) results in all shap values being 0.

To prevent having to run the entire notebook, I used python tool called 'dill'.

To load the session, in the last cell of the 'nlp_shap.ipynb' uncomment the command dill.load_session(filename) and comment the command 'dill.dump_session(filename)
(to save a session, leave the code as is).

