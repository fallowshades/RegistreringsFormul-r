# RegistreringsFormul-r

## copy

inspriation: https://colorlib.com/wp/free-bootstrap-registration-forms/

### skicka formulär

test request/response

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
  </head>
  <body>
    <section>

    <div class="form-center">
      <form action="https://httpbin.org/anything" method="post">
    <form action="submit.php" method="post">
      <label for="firstname" >first Name</label>
      <input type="name" id="text1" name="name" required/><br />


      <label for="firstname" >Last name</label>
       <input type="name" id="text1" name="name" required/><br />

      <label for="email">email</label>
      <input type="email" id="text2" name="email" /><br />

      <label for="password">Lösenord:</label>
      <input type="password" id="password" name="password" /><br />

      <label>Gender:</label><br />
      <input type="radio" id="radio1" name="male" value="male" />
      <label for="Male">Male</label><br />

      <input type="radio" id="radio2" name="female" value="female" />
      <label for="Female">Female</label><br />

      <label>order:</label><br />
      <input
        type="checkbox"
        id="checkbox1"
        name="mainDish"
        value="pasta"
      />
      <label for="checkbox1">pasta</label><br />

      <input
        type="checkbox"
        id="checkbox2"
        name="secondaryDish"
        value="tomatos"
      />
      <label for="checkbox2">tomatos</label><br />

      <input type="submit" value="Skicka" />
    </form>
    </div>
    </section>
  </body>
</html>


```

#### Hur ser textrutorna ut?

#### Vilket svar får du från lösenordsfältet?

"password": "secretDuckTape"

#### Försök välja en eller ett par av radioknapparna och skicka igen. Vad ändras?

"args": {},
"data": "",
"files": {},
"form": {
"email": "erik.jonsson@chasacademy.com",
"mainDish": "pasta",
"male": "male",
"name": [
"erik",
"jonsson"
],
"password": "secretDuckTape",
"secondaryDish": "tomatos"
},

#### Välj inga av radioknapparna och skicka.

{
"args": {},
"data": "",
"files": {},
"form": {
"email": "erik.jonsson@chasacademy.com",
"name": [
"erik",
"jonsson"
],
"password": "secretDuckTape"
},
"headers": {
"Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,_/_;q=0.8,application/signed-exchange;v=b3;q=0.7",
"Accept-Encoding": "gzip, deflate, br",
"Accept-Language": "sv-SE,sv;q=0.9,en-US;q=0.8,en;q=0.7",
"Cache-Control": "max-age=0",
"Content-Length": "83",
"Content-Type": "application/x-www-form-urlencoded",
"Host": "httpbin.org",
"Origin": "null",
"Sec-Ch-Ua": "\"Google Chrome\";v=\"117\", \"Not;A=Brand\";v=\"8\", \"Chromium\";v=\"117\"",
"Sec-Ch-Ua-Mobile": "?0",
"Sec-Ch-Ua-Platform": "\"Windows\"",
"Sec-Fetch-Dest": "document",
"Sec-Fetch-Mode": "navigate",
"Sec-Fetch-Site": "cross-site",
"Sec-Fetch-User": "?1",
"Upgrade-Insecure-Requests": "1",
"User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/117.0.0.0 Safari/537.36",
"X-Amzn-Trace-Id": "Root=1-65250665-5de2520a0462ca613eaa6708"
},
"json": null,
"method": "POST",
"origin": "155.4.199.114",
"url": "https://httpbin.org/anything"
}

#### Markera kryssrutorna och skicka.

{
"args": {},
"data": "",
"files": {},
"form": {
"email": "erik.jonsson@chasacademy.com",
"mainDish": "pasta",
"male": "male",
"name": [
"erik",
"jonsson"
],
"password": "secretDuckTape",
"secondaryDish": "tomatos"
},

#### Lämna kryssrutorna obestämda och skicka.

{
"args": {},
"data": "",
"files": {},
"form": {
"email": "erik.jonsson@chasacademy.com",
"name": [
"erik",
"jonsson"
],
"password": "secretDuckTape"
},
"headers": {
"Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,_/_;q=0.8,application/signed-exchange;v=b3;q=0.7",
"Accept-Encoding": "gzip, deflate, br",
"Accept-Language": "sv-SE,sv;q=0.9,en-US;q=0.8,en;q=0.7",
"Cache-Control": "max-age=0",
"Content-Length": "83",
"Content-Type": "application/x-www-form-urlencoded",
"Host": "httpbin.org",
"Origin": "null",
"Sec-Ch-Ua": "\"Google Chrome\";v=\"117\", \"Not;A=Brand\";v=\"8\", \"Chromium\";v=\"117\"",
"Sec-Ch-Ua-Mobile": "?0",
"Sec-Ch-Ua-Platform": "\"Windows\"",
"Sec-Fetch-Dest": "document",
"Sec-Fetch-Mode": "navigate",
"Sec-Fetch-Site": "cross-site",
"Sec-Fetch-User": "?1",
"Upgrade-Insecure-Requests": "1",
"User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/117.0.0.0 Safari/537.36",
"X-Amzn-Trace-Id": "Root=1-65250665-5de2520a0462ca613eaa6708"
},
"json": null,
"method": "POST",
"origin": "155.4.199.114",
"url": "https://httpbin.org/anything"
}

### Layout
