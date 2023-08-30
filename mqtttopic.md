## How do you design MQTT topics and payloads for smart washing machine

1. สถานะเครื่องซักผ้า
    - topic:v1cdti/app/get/6310301006/model-01/sn-001/
    - payload
        - {"STATUS": "POWER ON|START|STOP|FINISHED|POWERED OFF"}
1. เซนเซอร์ภายในเครื่องซักผ้า
    - topic:v1cdti/app/get/6310301006/model-01/sn-001
    - payload
        - {"temperature": "25.2"}
        - {"Humidity": "54"}
        - {"Time": "50"}
        - {"Airflow": "80"}
        - {"Cool_Down": "10"}
        - {"imbalance": "11"}
        - {"load": "5.4"}
        - {"water_level": "9"}
        - {"detergent": "50"}
        - {"noise_anomaly": "50"}
        - {"Rotating": "1000"}
        

 1. เซนเซอร์ภายนอกเครื่องซักผ้า
    - topic:v1cdti/app/get/6310301006/model-01/sn-001
    - payload
        - {"Lid sensor": "off"}
        - {"Vibration": "10"}
        - {"current": "110"}
        - {"Child_Lock": "off"}




