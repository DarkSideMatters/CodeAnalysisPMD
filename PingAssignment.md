
# Problem:
We want to test the ping time on 3 different servers to prove a relation between location and response time.

# Experiment setup:
We were given 3 different IP’s to connect to:

128.199.144.199
167.99.51.33
46.101.253.149

We checked those over https://www.iplocation.net/  to find out their locations and it gave us the following:


|IP |Location |    City|
|:---:|:---:|:---:|
|128.199.144.199  |   Singapore | Singapore|
|167.99.51.33   | USA - New Jersey  | Clifton|
|46.101.253.149 | Germany | Frankfurt am Main|



During the experiment we have two locations - Kongens Lyngby and Copenhagen City Center. To calculate the distance we used a most trusted source - Google Maps.

---------------------------------------

From Lyngby to Singapore: 9,966.85 km

From Lyngby to New Jersey: 6,178.43 km

From Lyngby to Frankfurt: 678.07 km

---------------------------------------

Copenhagen CC to Singapore: 9 964,11 km

Copenhagen CC to Clifton, New Jersey: 6,184.38 km

Copenhagen CC to Frankfurt: 670.03 km

---------------------------------------

Our expectations is that the Frankfurt point is going to have the fastest response time, opposed to Singapore, which is the farthest.



# Experiment:

Our experiment consists of pinging the server ips from the two different locations we have in order to make a conclusion. We have run the tests with the help of ping command in terminal.

---------------------------------------

**From Lyngby to different IPs:**

The First check was to Singapore. I pinged it 4 times and got between 203 and 204 ms.

The second check was to Clifton. I pinged it 4 times and got between 89 and 93 ms.

The Third check was to Frankfurt. I pinged it 4 times and got between 14 and 15 ms

---------------------------------------

**From Copenhagen CC to different IPs:**

The First check was to Singapore. Pinged 4 times and got between 179 and 184 ms.

The second check was to Clifton, NJ.  Pinged 4 times and got between 87 and 90 ms.

The Third check was to Frankfurt. Pinged 4 times and got between 16 and 50 ms.



# Evaluation:

According to the results we got from the 2 different places we tested from, we can safely say that our initial presumption for the speed is correct. Response time is related to distance. The more distance in between ips, the slower the response time.





# Discussion:

What we measure, how we measure and what could influence what influence our results.

What we measure is the ping time to the 3 different locations.

We measure it by pinging the different locations 4 times each, to get a more accurate estimation. We do this in the command prompt by writing: Ping xxx.xxx.xxx.xxx

What could influence our results is could be our internet speed, as it could cause delays and therefore higher response times. It could also be our destination. Time of the day (if the server is busy) could also be a huge factor to measuring the speed.


**_Made by Emil and Plamen._**
