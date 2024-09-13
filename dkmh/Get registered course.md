# Get Registered Course

Method: `POST`  
URL: `https://thongtindaotao.sgu.edu.vn/api/dkmh/w-locdskqdkmhsinhvien`  
Headers:  
 - `Content-Type`: `application/json`  
 - `Authorization`: `Bearer {access_token}`
 - `ua` : `{ua}`

Variables:  
 - `{access_token}` : Read [auth](../auth/Auth.md)
 - `{ua}`: Read [ua](../script/ua.md)

Body:  
 ```json
 {
    "is_CVHT": false,
    "is_Clear": false
 }
 ```

Response:  
 ```ts
 type RegiCourseResponse = {
  data: {
    total_items: number;
    total_pages: number;
    so_tin_chi_min: number;
    // ISO 8601 format
    ngay_in: string;
    is_show_nganh_hoc: boolean;
    ds_kqdkmh: {
        id_kqdk: string;
        trang_thai_mon: string;
        ngay_dang_ky: string;
        nguoi_dang_ky: "{username}_web";
        is_da_rut_mon_hoc: boolean;
        enable_xoa: boolean;
        dien_giai_enable_xoa: string;
        hoc_phi_tam_tinh: 0;
        to_hoc: {
          id_to_hoc: string;
          id_mon: string;
          ma_mon: string;
          ten_mon: string;
          so_tc: string;
          so_tc_so: number;
          is_vuot: boolean;
          nhom_to: string;
          lop: string;
          is_kdk: boolean;
          sl_dk: 0;
          sl_cp: 0;
          sl_cl: 0;
          tkb: string;
          is_hl: boolean;
          enable: boolean;
          hauk: boolean;
          is_dk: boolean;
          is_rot: boolean;
          is_ctdt: boolean;
          is_chctdt: boolean;
          is_kg_lt: boolean;
          thu: 0;
          tbd: 0;
          so_tiet: 0;
          is_kg_huy_kqdk: boolean
        }
      }[];
  };
  result: true;
  code: 200
}
 ```