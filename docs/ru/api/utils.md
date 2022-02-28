# Получение списка боссов # {: #bosses }
=== "TypeScript"

    ```typescript
    import { GenshinInfoClient } from 'genshin-info-api';
    await new GenshinInfoClient('TOKEN').getBosses({lang: "RU"})
    ```

=== "CURL"

    ```shell
    curl --location --request GET 'https://api.genshin-info.top/v1/bosses?lang=RU' \
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

# Получение информации рыбалки # {: #fishing }
=== "TypeScript"

    ```typescript
    import { GenshinInfoClient } from 'genshin-info-api';
    await new GenshinInfoClient('TOKEN').getFishingsplace({lang: "RU"})
    ```

=== "CURL"

    ```shell
    curl --location --request GET 'https://api.genshin-info.top/v1/fishing?lang=RU' \
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


