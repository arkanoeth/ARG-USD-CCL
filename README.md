# ARG-USD-CCL

I wrote this code back in 2020 to help me calculate the CCL in Argentina. Basically, it's a way to figure out the implied exchange rate between local stocks and their ADRs. To do this, I used financial information from Invertir Online and created a formula that multiplies the local stock price by a certain number and divides it by the ADR price.

The code then takes the stock quotes and CCL values it obtains and puts them into a table using a library called tabulate, which makes it easier to read and understand. Additionally, I used another library called matplotlib to create a bar chart that shows the CCL values for each local stock.

To get all this information, the code uses a special kind of authentication called OAuth2 to access InvertirOnline's API, which is how it gets the stock quotes.
