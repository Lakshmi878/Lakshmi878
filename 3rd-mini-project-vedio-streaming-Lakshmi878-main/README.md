# netflix_clone
A node express repo to demonstrate video stream

1. Setup:
    
    ```
    cd netflix_clone && npm install
    ```

2. Load data:
    1. Open your mongo shell
    2. Inside mongo shell

    - Create db with name `netflix_db`

    ```
    > use netflix_db
    ```

    - Load series data

    ```
    netflix_db> db.shell.insertMany([
        {
            title: '83',
            title_img: 'https://occ-0-2087-2164.1.nflxso.net/dnm/api/v6/LmEnxtiAuzezXBjYXPuDgfZ4zZQ/AAAABQPIgYvylQ4BYAWr1-T2yUiL-bOe7l5TaIVi5VXk48FXuLbVFspTbzo0mtjS-hBsImUScmR8NtdXCVyjtW4sule_bqThGvhnMFwq.webp?r=1c9',
            synopsis: "Amid doubt and derision, indomitable captain Kapil Dev leads India's struggling cricket team to make history at the 1983 World Cup. Based on true events.",
            banner: 'https://occ-0-2087-2164.1.nflxso.net/dnm/api/v6/6AYY37jfdO6hpXcMjf9Yu5cnmO0/AAAABZkf7Q9979J2jV2V7NjidxuLLLiC6zaD5UtV1wFofN07TVitnZSt9dOjYOMekeqI20_i_VYvm18DRs_nQ4sNZPDYM_7c.webp?r=c0d',
            ratings: '7.4',
            path: 'video.mp4'
        },
        {
            title: 'The Good Doctor',
            ratings: '8.2',
            small_banner: 'https://occ-0-2087-2164.1.nflxso.net/dnm/api/v6/X194eJsgWBDE2aQbaNdmCXGUP-Y/AAAABYQHx9Pd7krnBglmuVgJ29ypryT2XeYpB8aiFuQN27QR5i5hwT5hrdFJPQi9uwiDC3k5x1hOwpEmuecDXs830T47994.webp?r=65f',
            path: 'video.mp4',
            synopsis: 'The good doctor'
        },
        {
            title: 'Two and a half men',
            ratings: '8.2',
            small_banner: 'https://occ-0-2087-2164.1.nflxso.net/dnm/api/v6/X194eJsgWBDE2aQbaNdmCXGUP-Y/AAAABd9Yhh1hFJbDnaPNpEpSbYdLOiZCKXFiNJGE-TSj--olYWap0YySjWjQFGQKVd6Bl-IJTLok90wLqO115HYD_H1lcTc.webp?r=7c2',
            path: 'video.mp4',
            synopsis: 'Two and a half men'
        },
        {
            title: 'The Big Bang Theory',
            ratings: '8.2',
            small_banner: 'https://occ-0-2087-2164.1.nflxso.net/dnm/api/v6/X194eJsgWBDE2aQbaNdmCXGUP-Y/AAAABfhRpIbg2DZXb2Kur0OFqqqLOQ55ZX8lfLulyABdd5GWHp6GJdP_qA3Ag52UVs2I9CaRsICGHlK-qVVfOAxrRanEQX0.webp?r=9d9',
            path: 'video.mp4',
            synopsis: 'The Big Bang Theory'
        },
        {
            title: 'Brooklyn Nine-Nine',
            ratings: '8.2',
            small_banner: 'https://occ-0-2087-2164.1.nflxso.net/dnm/api/v6/X194eJsgWBDE2aQbaNdmCXGUP-Y/AAAABQO417AoaMguF_DtQ1zOivjKkMZEpP5zA1YFG1zwSewxnHSW3UyRVVbIUbhMdVsXnZzFolmiO9x3tteyklzoM_fZ9VA.webp?r=a8a',
            path: 'video.mp4',
            synopsis: 'The good doctor'
        },
        {
            title: "Schitt's Creek",
            ratings: '8.2',
            small_banner: 'https://occ-0-2087-2164.1.nflxso.net/dnm/api/v6/X194eJsgWBDE2aQbaNdmCXGUP-Y/AAAABc30tY_YHFejNG-KnOz0arx2aNm-aP694iyqyjkm1GJNeBalqlz6wnSAzQfOamq6NE5Sen5b7Fp5_hvVzzcpMCx9yOU.webp?r=a1d',
            path: 'video.mp4',
            synopsis: "Schitt's Creek"
        },
        {
            title: 'Seinfeld',
            ratings: '8.2',
            small_banner: 'https://occ-0-2087-2164.1.nflxso.net/dnm/api/v6/X194eJsgWBDE2aQbaNdmCXGUP-Y/AAAABdVd3EAjZkILBRyD0SBWeH3gLSlotpYxr7AK7bd3THaNGQ9KVJLJB5LSrAoJpZGlsrLrubxZXCqQ0Uzd2lT7DI9fsFA.webp?r=a2d',
            path: 'video.mp4',
            synopsis: 'Seinfeld'
        }]);

    ```





3. Start server:

    ```
    npm start
    ```

4. Open `localhost:8888` on your browser
