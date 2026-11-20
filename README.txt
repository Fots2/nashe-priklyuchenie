Наше маленькое приключение — публикация в Vercel

Это статический сайт без сборки. Главный файл: public/index.html.
Файл vercel.json явно указывает Vercel на папку public.
Копия index.html есть также в корне для других вариантов размещения.

Публикация через Vercel Drop:
1. https://vercel.com/drop
2. Загрузите ZIP целиком, выберите название проекта и Deploy.
3. После завершения нажмите Visit или откройте адрес из Deployments.

Публикация через GitHub и существующий проект Vercel:
1. Распакуйте ZIP и скопируйте index.html, public/index.html и vercel.json в корень репозитория.
2. В Vercel: Settings > Build and Deployment: Framework Preset Other, Root Directory . / корень репозитория, Build Command пусто, Output Directory public (совпадает с vercel.json).
3. Сделайте новый commit, дождитесь статуса Ready, откройте адрес из вкладки Domains.

Если снова 404: откройте Deployment > Output и убедитесь, что есть index.html. Также проверьте, что домен назначен последнему Production deployment.

Для анимированной GIF Tenor в финале нужен интернет; при его отсутствии показывается резервная картинка.
