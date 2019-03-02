FORMAT: 1A
HOST: http://pc.stmikbumigora.ac.id/

# Programing Comunity Bumgora 

Registrasi member Programing Comunity 

## Register Member [/member/]

### Create a New Member [POST]

You may create your own question using this action. It takes a JSON
object containing a question and a collection of answers in the
form of choices.

+ Request (application/json)

        {
            "name": "zillu"
        }

+ Response 201 (application/json)

    + Headers

            Location: /member

    + Body

            {
                "respone": "succes created member",
            }

## Member GET All [/member]

### List All Member [GET]

+ Response 200 (application/json)

        [
            {
                "id": 1,
                "name": "ulul azmi"
            },
            {
                "id": 2,
                "name": "RIZKA RAHMAWATI"
            },
            {
                "id": 3,
                "name": "yan"
            },
            {
                "id": 4,
                "name": "zillu"
            }
        ]

## Member GET First [/member/1]

### Get First Member [GET]

+ Response 200 (application/json)
    
    + Body

            {
                "id": 1,
                "name": "ulul azmi"
            }
