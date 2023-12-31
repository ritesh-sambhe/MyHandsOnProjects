# Transit Gateway Creation within NV & Oregon Region

![image](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/27ac18ea-ba4d-4c70-9c91-662e78a37d33)

![image](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/b8657008-652e-48e6-8cd2-e058fc5996a5)

![image](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/8a5238a2-1812-451f-bf3b-85c227ee7e30)

![image](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/f21b84ca-e87c-4cc3-b3f6-29aae52ebea3)

![image](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/28f11ff1-1e3c-45cf-a60b-a4ba41453d0f)

# Similarly Create VPC,IGW, ROUTE Table, Subnet for second Region to connect with like Oregon I chose to created in this case.

# Now Creating TGW, TGW Attachment for VPC type, TGW Attachment for Peering Connection type and Transit-GW RouteTable, in North Verginia.

![image](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/581476cd-0479-4178-b83e-dc1617f498bb)

![image](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/85bccb48-b160-4bdb-b5d8-ecf4c9e4efa3)

#Initiated Peering request from North Verginia to Oregon
![image](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/a170b912-4953-424a-a273-de6aa85e382f)
![image](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/d4f4054b-fd77-4d0b-aafa-11e6b68d7b5f)

#Accepted the TGW attachment Peering Connection which is Initiated from NV & Accepted at Oregon
![image](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/fc0597ad-880c-418b-9e9b-8a946a06c526)

#Add static route in TGW route table (NV)
![image](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/ddcacf2f-89ba-4ac3-83a3-722eaca657cd)

#Add static route in TGW route table (Oregon)
![image](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/41266424-c8de-497e-9edb-4d6c73aceecf)

#Instances of NV and Oregon Rgion.
![image](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/c488769a-2275-4196-898b-a77486a2ee15)

![image](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/89b79229-ca54-4c6f-bd94-ff0b880306bf)



# RESULT at NV EC2 Instance Trying to Ping Oregon Instance using PrivateIP address
![image](https://github.com/ritesh-sambhe/MyHandsOnProjects/assets/144586067/dac494e0-3850-4468-aa9e-7093fbded8f3)
