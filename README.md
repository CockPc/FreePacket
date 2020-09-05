# FreePacket

프로토콜에 따라서 프로그램을 짜다보면 생략되는 부분이 너무 많아서 가끔은 왜 안돌아가는지 알 수 없을 때가 있다
이미 충분히 OS가 그걸 생략하고 있는데 클라이언트단에서도 생략해버리면 나는 좀 힘들다

그래서 Packet based 로 접근하려고 한다 사실 하다보니 PACKET BASED로 됬는데 또 모른다

Message란 로그인 정도가 있다 파일도 FTP를 써서 구현 해볼 수도 있다 

class Message{
	public:
	char name[20];
	enum status
	void generate_packets_list(name)
	{
		switch (name)
		case LOGIN:
			map(LOGIN_OKAY).insert(PACKET<-gen_pack(LOGIN.OKAY));
			map(LOGIN_ADDRESS).insert(PACKET<-gen_pack(LOGIN.ADDRESS));
			map(LOGIN.START).insert(PACKET<-gen_pack(LOGIN.START);
			
      map(LOGIN.START).send();                      //             recv makepacket reply 
      map(LOGIN.START).recv();
      if(map(LOGIN.START).validate(recv_packet))? map(LOGIN.START).update_status():return;
      if(map(LOGIN.START).status == "SUCCESS")? {map(LOGIN_ADDRESS).insert(PACKET); }:return;
  }
};
enum Status { 
  STATUS_OKAY,
  STATUS_LOGIN,
  STATUS_ACK,
  STATUS_FAIL
};
  
Status status = STATUS_OKAY;
