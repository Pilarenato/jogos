# jogos
Desenvolvimento de jogos 3D
Docs

API Endpoint: https://miami-hackathon.herokuapp.com
User
Login

  [GET] /auth/facebook?fb_token={FACEBOOK_ACCESS_TOKEN}

Example (need to use and software to POST):

https://miami-hackathon.herokuapp.com/auth/facebook?fb_token=CAAXiYjEPaTMBAHReQKnncXZBmX6hZAbcthEdECCB9eeL4JKWQXkLjZCAZAo0uUSYcjkZCtFoZAIojeuZCjeE0BKj42RwDO76u8ZAkZARZBVS789ahyZBbMRWqcJH8BgkZAWK1jckWnqyMV4T9r8KK8WJs79Vz6OJ26JFWoEPAWZALMUn5O8AZBQnSCZAuGNO3extrkKZCOe024ZANEjHYXAZDZD

Details

  [GET] /user?access_token={ACCESS_TOKEN}

Example:

https://miami-hackathon.herokuapp.com/user?access_token=hMGGWwAOWHKvE/rB4h7uksMoIxOSqV2D7QFBZEeQ4PGmsa2i3eTIKWs1ktos7iAyTv40Df0lPLe5cM/gK3lAMg==

Update / Simplify Commerce

  [GET] /user?name={NAME}&email={EMAIL}&creditCardToken={SIMPLIFY_COMMERCE_TOKEN}&access_token={ACCESS_TOKEN}

Medicines

  [GET] /user/medicines?access_token={ACCESS_TOKEN}

This will associate an existent medicine with a user:

  [POST] /user/medicines?medicineId={NAME}&access_token={ACCESS_TOKEN}

This will create a medicine and associate with a user:

  [POST] /user/medicines?name={NAME}&picture={PICTURE_URL}&access_token={ACCESS_TOKEN}

Example:

https://miami-hackathon.herokuapp.com/user/medicines?name=Novalgina&access_token=hMGGWwAOWHKvE/rB4h7uksMoIxOSqV2D7QFBZEeQ4PGmsa2i3eTIKWs1ktos7iAyTv40Df0lPLe5cM/gK3lAMg==

Prescriptions
List

  [GET] /user/prescriptions?access_token={ACCESS_TOKEN}

  [POST] /user/prescriptions?userMedicineId={MEDICINE_ID}&weekDay={WEEK_DAY}&dayTime={DAY_TIME}&repeatUntil={REPEAT_UNTIL_DATE}&access_token={ACCESS_TOKEN}

Medicines
List

  [GET] /medicines

  [POST] /medicines?name={NAME}&picture={PICTURE_URL}
