# Получение всего списка персонажей # {: #charteres }
=== "TypeScript"

    ```typescript
    import { GenshinInfoClient } from 'genshin-info-api';
    await new GenshinInfoClient('TOKEN').getCharacters({lang: "RU"})
    ```

=== "CURL"

    ```shell
    curl --location --request GET 'https://api.genshin-info.top/v1/characters?lang=RU' \
    --header 'Authorization: TOKEN'
    ```

Ответы сервера:

=== "200"

    ```json
    ответ
    ```

=== "404"

    ```json
     {statusCode: 404, message: "Notfound"}
    ```

# Получение информация о персонаже # {: #charterer}
=== "TypeScript"

    ```typescript
    import { GenshinInfoClient } from 'genshin-info-api';
    await new GenshinInfoClient('TOKEN').getCharacter({lang: "RU", name: "Дилюк"})
    ```

=== "CURL"

    ```shell
    curl --location --request GET 'https://api.genshin-info.top/v1/character?lang=RU&name=Дилюк' \
    --header 'Authorization: TOKEN'
    ```

Ответы сервера:

=== "200"

    ```json
    ответ
    ```

=== "404"

    ```json
     {statusCode: 404, message: "Notfound"}
    ```


