
    # Instructions for Testing Deep Neural Network and Linear Regression Models

    This notebook allows you to test the performance of various DNN models and a Linear Regression model on the provided test dataset.
    
    ## Pre-requisites:
    - Ensure all models (DNN-16, DNN-30-8, DNN-30-16-8, DNN-30-16-8-4, and Linear Regression) are trained.
    - Test features (X_test_scaled) and test labels (y_test) should be available and preprocessed before testing.

    ## Steps to Test Models:
    1. After running all cells, the function `run_tests_on_all_models()` will automatically test the performance of the following models:
       - DNN-16
       - DNN-30-8
       - DNN-30-16-8
       - DNN-30-16-8-4
       - Linear Regression

    2. Each model is tested on the test dataset, and the following metrics are displayed:
       - R-squared (R²) score
       - Mean Squared Error (MSE)

    3. Additionally, a scatter plot comparing the actual vs. predicted values of the target variable will be shown for each model.
    
    ## Custom Testing:
    If you want to test individual models, you can call the respective testing function for each model:
    
    - For DNN models:
    
    ```
    test_model_dnn(model, X_test_scaled, y_test, model_name)
    ```
    
    Example:
    
    ```
    test_model_dnn(dnn_model_16, X_test_scaled, y_test, "DNN-16")
    ```

    - For Linear Regression model:
    
    ```
    test_model_linear(lr_model, X_test_scaled, y_test, model_name)
    ```

    Example:
    
    ```
    test_model_linear(lr_model, X_test_scaled, y_test, "Linear Regression")
    ```

    ## Contact
    For any issues or further clarifications, please contact the notebook author.
    