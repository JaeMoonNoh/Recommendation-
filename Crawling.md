# Crawling description

1. from selenium import webdriver
2. data = request.get('네이버웹툰사이트')
3. soup = BeautifulSoup(data,'html.parser')


4. title = soup.find_all('a',{'class':'title'})


