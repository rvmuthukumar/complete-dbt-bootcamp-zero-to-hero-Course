
# Key creation 
    - https://docs.snowflake.com/en/user-guide/key-pair-auth
    
# Creating private key
openssl genrsa 2048 | openssl pkcs8 -topk8 -v2 des3 -inform PEM -out rsa_key.p8
q

# creating public key 
openssl rsa -in rsa_key.p8 -pubout -out rsa_key.pub
q
