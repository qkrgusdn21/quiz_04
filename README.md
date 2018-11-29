Quiz 04
=

모든 퀴즈는 해당 강의중에 언급된 내용에서만 국한된다.  
퀴즈 답변이 모호하다고 생각한다면 해당 이유를 적고 본인이 생각하는 답을 작성하여 제출한다.  

0_1. 해당 퀴즈 git을 fork하여 답안을 작성하시오.  
0_2. 운영진의 공지를 확인하고 알맞은 branch로 답지를 pull request를 보내시오.  
1. follow 기능을 어떤 gem으로 구현하였는가?  
    답 : acts_as_follower 젬
2. Comment 모델과 N:M 관계를 가지는 모델을 전부 쓰시오  
    답 : 
3. profile 유효성검사는 어떻게 하였는지 적으시오  
    답 : validates :name, presence: true, length: { minumum:1, maximum: 30}
        이런 식으로 적고 유효성 검사하고 싶으면 p.valid? 이런 식으로.
4. 커스텀 helper를 사용한 기능은 무엇인지 모두 쓰시오  
    답 : form_for, link_to
5. 파일 업로더는 어떤 방식으로 구현하였는가  
    답 : carrierwave, fog_aws, mini_magick gem 으로 구현하였다.
6. controller 중 rendering view 로만 이루어진것은 무엇인지 모두 쓰시오   
    답 : show, edit
7. 강의중 게시글 본문의 에디터는 어떻게 구현하였는지 쓰시오  
    답 : 
8. 댓글은 어떻게 구현하였는지 쓰시오   
    답 : 게시글 테이블과 1:N 관계를 구성 
         모델에서 post.rb 파일에는 has_many :comments, comment.rb파일에는 belongs_to :post 해주면 관계 성립
9. 컨트롤러로 넘어오는 입력값을 어떻게 가공하여 모델로 넘겨주는지 쓰시오  
    답 :  Params.require(:article).permit(:title, :content) 이런 식으로 require 쓰고 permit
10. 프로젝트의 root_url은 어디로 연결되어있는지 쓰시오
    답 : home index
11. article_url 의 method : get 요청에는 몇개의 html 페이지가 렌더링되있는지 적고 각각이 어떤 redering page 인지 적으시오  
    답 : 

12. 본인의 보조강의 워크스페이스 github repo 주소를 적으시오  
깃헙에 없다면 새로 만들어서 링크를 제출하시오   
    답 : 코드스타 세션 마치고 실수로 ec2 인스턴스 삭제해서 없어졌어요..