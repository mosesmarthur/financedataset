import joblib
import json

def predict(event, context):
    # Load the serialized Random Forest model from s3
    model = joblib.load('random_forest_model.pkl')

    # Get the input data from the request
    input_data = json.loads(event['body'])

    # Perform prediction
    prediction = model.predict(input_data)

    # Return the prediction as JSON
    return {
        'statusCode': 200,
        'body': json.dumps({'prediction': prediction.tolist()})
    }
