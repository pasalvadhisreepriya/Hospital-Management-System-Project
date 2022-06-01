package com.hospital;

import java.io.IOException;
import javax.servlet.ServletException;
import javax.servlet.annotation.WebServlet;
import javax.servlet.http.HttpServlet;
import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletResponse;
import javax.servlet.http.HttpSession;


@WebServlet(urlPatterns="/AdminLogin")
public class AdminLogin extends HttpServlet {
	private static final long serialVersionUID = 1L;
       

    public AdminLogin() {
        super();
    }
    
	protected void doGet(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {
		response.getWriter().append("Served at: ").append(request.getContextPath());
		
	}

	protected void doPost(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {
		HttpSession session=request.getSession();
		String name=request.getParameter("username");
		String psswd=request.getParameter("password");
		if(name.equalsIgnoreCase("Sreepriya")&&psswd.equalsIgnoreCase("Sree@1221"))
		{			session.setAttribute("id",1);		
			request.getRequestDispatcher("AdmPage.jsp").forward(request, response);
		}
	
		else {
			request.setAttribute("error", "Invalid username/password.");
			request.getRequestDispatcher("AdmLogin.jsp").forward(request, response);
	}
	}
}