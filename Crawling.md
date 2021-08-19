# Crawling description

# 1. from selenium import webdriver
# 2. data = request.get('네이버웹툰사이트')
# 3. soup = BeautifulSoup(data,'html.parser')
![html_](https://user-images.githubusercontent.com/62277037/130057480-e82524bf-fd74-4171-9fbd-b84a8787748f.PNG)

# 4. title = soup.find_all('a',{'class':'title'})
![타이틀만뽑아오기](https://user-images.githubusercontent.com/62277037/130057085-f9d0ce0c-a5a2-4b48-8549-b18a892bba02.PNG)

# 5. 타이틀 뽑은 결과
![타이틀_뽑은_결과](https://user-images.githubusercontent.com/62277037/130057511-e8a006ae-5cb1-4e73-a695-ac3437371d69.PNG)
# 6. day = soup.find_all('ul', {'class' : 'category_tab'}) , day = day[0].find('li', {'class' : 'on'}).text[0:1]
![네이버웹툰크롤링 페이지클릭하면서데이터수집](https://user-images.githubusercontent.com/62277037/130057512-0e40754e-08c1-482a-b818-cecf59085676.PNG)
# 7. 장르 줄거리 작가
![네이버웹툰크롤링 줄거리,장르](https://user-images.githubusercontent.com/62277037/130057516-7a14a23c-8226-4dc5-8159-1b8713a28ce2.PNG)
# 8. 결과

