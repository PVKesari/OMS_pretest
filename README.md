Executing jar
java -jar pretest-0.0.1-SNAPSHOT

Post Request
 http://localhost:8088/getOrderDetails

Request Body
{
"orderId":"Order1"
}

Response Body

{
    "order": [
        {
            "orderId": "Order1",
            "productId": "Prod1",
            "qty": 2.0
        }
    ],
    "shipment": [
        {
            "orderId": "Order1",
            "shipmentId": "Ship1",
            "productId": "Prod1",
            "shipmentDate": "1970-01-01T00:00:02.000+00:00",
            "qty": 2.0
        }
    ]
}

Post Request 
http://localhost:8088/getAvailability

Request Boby
{ "productId":"Product1"}

Response Body
{
    "productId": "Product1",
    "availability": 8.0
}
