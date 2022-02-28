# Получение всех артефактов # {: #arts }
=== "TypeScript"

    ```typescript
    import { GenshinInfoClient } from 'genshin-info-api';
    await new GenshinInfoClient('TOKEN').getArts({lang: "RU"})
    ```

=== "CURL"

    ```shell
    curl --location --request GET 'https://api.genshin-info.top/v1/arts?lang=RU' \
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

# Получение информация о артефакте # {: #art }
=== "TypeScript"

    ```typescript
    import { GenshinInfoClient } from 'genshin-info-api';
    await new GenshinInfoClient('TOKEN').getArt({lang: "RU", name: "алая ведьма"})
    ```

=== "CURL"

    ```shell
    curl --location --request GET 'https://api.genshin-info.top/v1/art?lang=RU&name=алая ведьма' \
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


