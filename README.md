Работа с git и bash
-
2. cd /Users/alexey.larchenko/documents/BASH
3. pwd
4. mkdir test1
5. cd test1
6. touch 1 2 3
7. ls
8. cd ..
9. mkdir test2 
10. rmdir test2
11.  rm ./test1/2
12. mkdir test3
      touch ./test3/1 ./test3/2  
13. rm -rf test3
14. mkdir test4
15. mv ./test1/1 ./test1/3 test4/ 
16. echo -e "line\nline\nline" >> ./test4/1
17. cat ./test4/1
18. echo -e "line\nline\nline" >> ./test4/3
19. cat ./test4/1 ./test4/3
20. nano ./test4/1
-
2.  cd /Users/alexey.larchenko/documents/BASH
3. mkdir test3
4. touch  ./test3/4 ./test3/5 ./test3/6 
    echo -e "row1\nrow2\nrow3\nrow4" >> ./test3/4 >> ./test3/5 >> ./test3/6
5. grep "row2" ./test3/5
6. find ./test3 h -type f -exec grep "row" {} \;  
7. grep "row" ./test3/6 -c 
8. find ./test3 -name "5"
9. find . -type f -name "5" -exec rm -f {} \;
10. echo "test" >> ./test3/4 
11. sed -i -e 's/test/fail/' ./test3/4
12. echo "test" >> ./test3/4
13. ps aux
14. kill 666
15. ping rusau.net
16. ping -c 3 rusau.net
17. curl -X 'GET' \
  'https://petstore.swagger.io/v2/pet/findByStatus?status=available&status=pending&status=sold' \
  -H 'accept: application/json'
18.curl -X 'POST' \
  'https://petstore.swagger.io/v2/pet' \
  -H 'accept: application/json' \
  -H 'Content-Type: application/json' \
  -d '{
  "id": 31232,
  "category": {
    "id": 1,
    "name": "dog"
  },
  "name": "doggie",
  "photoUrls": [
    "https://www.google.com/url?sa=i&url=https%3A%2F%2Fmalinois.com.ua%2Fru%2F2020%2F11%2F11%2Fno-breed-dog-review%2F&psig=AOvVaw1fD-ymBnvONIxVdKk2_irF&ust=1729414173600000&source=images&cd=vfe&opi=89978449&ved=0CBQQjRxqFwoTCIDR_f2HmokDFQAAAAAdAAAAABAE"
  ],
  "tags": [
    {
      "id": 5,
      "name": "gav"
    }
  ],
  "status": "available"
}'
