# Starbucks-backend
one Starbucks-backend


public DNS name: ec2-54-183-201-12.us-west-1.compute.amazonaws.com

port: 9090


Place order API: (Method: POST, will return ORDER_ID)
http://54.183.201.12:9090/v3/starbucks/order

Info needed:
    { "location": "take-out",
      "items": [{
      "qty": 1,
      "name": "latte",
      "milk": "whole",
      "size": "large"
    }]}


Pay API: (Method: POST)
http://54.183.201.12:9090/v3/starbucks/order/{ORDER_ID}/pay


Get order API: (Method: GET)
http://54.183.201.12:9090/v3/starbucks/order/{ORDER_ID}


Delete order API:(Method: DELETE)
http://54.183.201.12:9090/v3/starbucks/order/{ORDER_ID}


Update order API:(Method: PUT)
http://54.183.201.12:9090/v3/starbucks/order/{ORDER_ID}

Info needed:
    { "location": "take-out",
      "items": [{
      "qty": 1,
      "name": "latte",
      "milk": "skim",
      "size": "small"
    }]}
