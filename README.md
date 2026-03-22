 Telemetry Data Converter

 Overview
This project is a Python-based solution designed to convert telemetry data from multiple JSON formats into a unified structure. It ensures consistency in data representation, making it easier for further processing, analysis, and monitoring.

In real-world systems such as IoT devices and industrial machines, data is often received in different formats. This project demonstrates how to standardize such data efficiently.

---

 Features
- ✅ Supports multiple input JSON formats  
- ✅ Converts ISO timestamp to milliseconds (epoch time)  
- ✅ Produces a unified output format  
- ✅ Includes automated test validation  
- ✅ Simple and easy-to-understand implementation  

---

 Project Structure
```
telemetry-project/
│── data-1.json        # Input format 1
│── data-2.json        # Input format 2
│── data-result.json   # Expected unified output
│── main.py            # Conversion logic + test cases
```

---

 How It Works

The project processes two different telemetry formats:

### 🔹 Format 1
- Uses ISO timestamp (e.g., `2023-10-01T12:00:00Z`)
- Keys like `deviceId`, `temperature`, `humidity`

### 🔹 Format 2
- Uses Unix timestamp (seconds)
- Different key names like `id`, `temp`, `hum`

Conversion
Both formats are converted into a common structure:

```json
{
  "device_id": "abc123",
  "timestamp": 1696161600000,
  "temperature": 25,
  "humidity": 60
}
```

---

 How to Run

### Requirements
- Python 3.x

### Steps
```bash
python main.py
```

Output
```
All tests passed!
```

---

Testing
The project includes built-in test cases that:
- Validate both input formats
- Compare output with expected results
- Ensure accuracy of conversion logic

---

 Technologies Used
- Python
- JSON

---

 Use Cases
- IoT data processing  
- Machine telemetry monitoring  
- Data standardization pipelines  
- Backend data transformation systems  

---

 Author
- Hamsini Govvala

---

 Conclusion
This project demonstrates how to handle and standardize inconsistent data formats, a common challenge in real-world software systems. It highlights the importance of data transformation in building scalable and reliable applications.
