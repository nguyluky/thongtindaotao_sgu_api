# Get Notification

Method: `POST`  
URL: `https://thongtindaotao.sgu.edu.vn/api/web/w-locdsthongbao`  
Headers:  
 - `Content-Type`: `application/json`  
 - `Authorization`: `Bearer {access_token}`

Variables:  
 - `{access_token}` : Read [auth](auth.md)

Body:  
 ```json
 {
    "filter": {
        "id": null,
        "is_noi_dung": !0
    },
    "additional": {
        "paging": {
            "limit": 100,
            "page": 1
        },
        "ordering": [{
            "name": "ngay_gui",
            "order_type": 1
        }]
    }
}
 ```

Response:  
 ```ts
type NotificationResponse = {
  data: {
    total_items: number;
    total_pages: number;
    notification: number;
    ds_thong_bao: {
      id: string;
      doi_tuong_search: string;
      doi_tuong: number;
      phan_cap_search: string;
      phan_cap_sinh_vien: number;
      tieu_de: string;
      noi_dung: string;
      is_phai_xem: boolean;
      ngay_gui: Date;
      is_da_doc: boolean;
      ds_doi_tuong: any[];
    }[];
  };
  result: boolean;
  code: number;
};

 ```

