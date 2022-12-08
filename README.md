# Java_Rule
#자바의 정석 예제 15-4 

# 문제
커맨드라인으로 부터 여러 파일의 이름을 입력받고 이 파일들을 순서대로 합쳐 ,
서 새로운 파일을 만들어 내는 프로그램(FileMergeTest.java) . , 을 작성하시오 단 합칠 파일 개수에는 제한을 두지 않는다.




# 결과코드
USAGE: java FileMergeTest MERGE_FILENAMEFILENAME1 FILENAME2 ...


# 해설
여러개의 파일을하나로 연결할때는 SequenceInputStream이 적합
 SequenceInputSt의 사용 예
 Vector files = new Vector();
files.add(new FileInputStream("file.001"));
files.add(new FileInputStream("file.002"));
SequenceInputStream in = new SequenceInputStream(files.elements());
