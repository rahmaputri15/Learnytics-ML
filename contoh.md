from flask import Flask, jsonify, request
import pandas as pd
from sklearn.cluster import KMeans

app = Flask(**name**)

@app.route('/predict/<student_id>', methods=['GET'])
def predict_recommendations(student_id): # Load student data # Apply ML model (clustering, prediction, etc.) # Return recommendations

    recommendations = [
        {"type": "focus", "module": "Dynamic Programming", "reason": "ML detected weak pattern"},
        {"type": "practice", "module": "Graph Theory", "reason": "Below cluster average"}
    ]

    return jsonify({"studentId": student_id, "recommendations": recommendations})

if **name** == '**main**':
app.run(port=5000)
