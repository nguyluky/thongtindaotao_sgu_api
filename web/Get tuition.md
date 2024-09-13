# Get tuition

Get tuition for each semester

Method: `POST`  
URL: `https://thongtindaotao.sgu.edu.vn/api/web/w-locdsthongbao`  
Headers:  
 - `Content-Type`: `application/json`  
 - `Authorization`: `Bearer {access_token}`
 - `ua` : `{ua}`


Variables:  
 - `{access_token}` : Read [auth](../auth/Auth.md)
 - `{ua}`: Read [ua](../script/ua.md)


Response:  
 ```ts
type TuitionResponse = {
  data: {
    total_items: number;
    total_pages: number;
    is_tinh_tong: boolean;
    is_show_hoc_bong: boolean;
    is_tg_dong_hoc_phi: boolean;
    is_hvsg: boolean;
    ds_hoc_phi_hoc_ky: {
      ten_nhom_ct: string;
      ten_hoc_ky: string;
      hoc_phi: string;
      mien_giam: string;
      phai_thu: string;
      tong_hoc_bong: string;
      da_thu: string;
      con_no: string;
      ghi_chu: string;
    }[];
    is_dong_hp_theo_edubill: boolean;
    url_edubill_gateway: string;
    messsage_error_edubill: string;
    url_call_api: string;
  };
  result: boolean;
  code: number;
};

 ```

